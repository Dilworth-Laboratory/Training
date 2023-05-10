# Data Management  
  
## Archiving  
  
Raw reads fastq.gz files, processed bigwigs, bed, and other genome coverage files from experiment results should all be <ins>backed up for archiving</ins>.  
Currently, this location is the <ins>**WISC ResearchDrive**</ins>, please contact the appropriate person to transfer any new data and keep this updated.  

Additionally, feel free to maintain your own data backed up as a redundancy which you can also manipulate for analysis.  

___  

## Access and Visibility  

&nbsp;&nbsp;&nbsp;&nbsp;For accessing experiment bigwigs and/or bed files, <a href="https://www.cyverse.org/">CyVerse</a> is used to <strong>*host*</strong> the data.  
&nbsp;&nbsp;&nbsp;&nbsp;The <a href="https://genome.ucsc.edu/">UCSC Genome Browser</a> connects to CyVerse to <strong>*display*</strong> the data.  
  
  
<strong>Accessing CyVerse Data:</strong>  
You may obtain access to Jeff Dilworth's CyVerse account with his permission, or create a free account; however, Jeff's account also acts as a redundant central location for archived data to be viewable.  
<ol>
  <li>Go to https://www.cyverse.org/ and in the nagivation bar click the "Sign up" drop-down, then click Log in</li>  
  <li>Launch Discovery Environment under "My Services"</li>  
  <li>Click on Data in the left navigation panel</li>  
  <li>Click the drop-down menu, change Community Data to Home (will be prompted to click Sign In)</li>
</ol>  
  
  
<strong>Viewing tracks in the UCSC Browser:</strong>  
A UCSC account is not required, but allows convenience to save connected hubs and sessions for viewing hubs/tracks anytime without having to set them up again.  
<ol>
  <li>Go to https://genome.ucsc.edu/ and in the navigation bar hover over My Data, then click Track Hubs in the drop-down</li>  
  <li>Click the Connected Hubs tab</li>  
  <li>Copy/paste your hub.txt URL link into the URL space and click Add Hub (you will be redirected to the home page)</li>  
  <li>Repeat steps 1 & 2, then click on the hub assembly</li>  
  <li>Scroll down and hide/show tracks for viewing, change display properties, explore viewing options, etc...</li>  
</ol>  
  
<center><img src="view_hubs_ucsc.png" alt="view_hubs_ucsc"/></center>  
  
  
## Conventions  
  
Typical steps after processing reads to view:  
<ol>  
  <li>Upload bigwig/bed files to CyVerse in appropriate locations (follow conventions, see below)</li>  
  <li>Create/update trackDb.txt, genomes.txt, hub.txt files</li>  
  <li>Connect hub.txt public link to UCSC browser</li>  
  <li>View data</li>  
</ol>  

The example hub.txt, genomes.txt, and trackDb.txt files in this repo can be used as a template for any new hubs or updating current ones.  
You should review the <a href="https://www.genome.ucsc.edu/goldenPath/help/hgTrackHubHelp.html">UCSC documentation for track hubs</a>.  

The current convention for hub organization on CyVerse is:  
<ul style="list-style-type: none;">  
  <li>LabsData/</li>  
    <ul style="list-style-type: none;">  
      <li>SampleType/<li>  
      <ul style="list-style-type: none;">  
        <li>genome.txt</li>  
        <li>hub.txt</li>  
        <li>assembly/</li>  
        <ul style="list-style-type: none;">
          <li>trackDb.txt</li>  
          <li>CUT&Tag/</li>  
          <li>RNASeq/</li>  
          <li>ChIPSeq/</li>  
          <ul style="list-style-type: none;">
            <li>ResearcherInitials/</li>  
            <ul style="list-style-type: none;">
              <li>chipdata1.bw</li>  
              <li>chipdata2.bw</li>  
            </ul>
          </ul>
        </ul>
      </ul>
    </ul>
</ul>

