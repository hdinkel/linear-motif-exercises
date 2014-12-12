linear-motif-exercises
======================

Linear motif biology, prediction, and cooperativity in cellular signalling

Objective: Get familiar with the [Phospho.ELM](http://phospho.elm.eu.org) resource. {#toc0}
===================================================================================

Searching via protein id {#toc1}
------------------------

1.  Go to [Phospho.ELM](http://phospho.elm.eu.org) and enter protein
    accession ‘CASP9_HUMAN’ in the second form field.
    1.  How many annotated sites/residues do you find? Which site have
        information from multiple references?
    2.  How many are annotated as ”high throughput experiments”?
    3.  What information is given on the surface accessibility of the
        annotated residues?
    4.  (Optional) later during this course, when you’ve learned to use
        a 3D-viewer, use it to visualize the structure of (
        [1NW9](http://www.rcsb.org/pdb/explore/explore.do?structureId=1NW9)
        ) and try to highlight the individual phosphorylatable residues
        and investigate their surface accessibility.

2.  Query Phospho.ELM for phosphorylation sites of protein ‘Cyclin
    dependent kinase inhibitor 1B’ CDN1B_HUMAN (use the accession
    P46527)
    1.  How many phosphorylation sites are annotated for this protein?
    2.  Which sites are well conserved as well as reside in disordered
        region? (Tip: Click the column heads for sorting)
    3.  Are there any (MINT) interactions annotated for this protein?
    4.  (OPTIONAL) Which of these interactions at MINT describe the
        phosphorylation reaction?

3.  Query Phospho.ELM for SRRM2_HUMAN to see a protein with a quite
    high number of phosphorylations. (Don’t) try to count them.
    1.  How many of these annotations stem from low throughput
        experiments?

* * * * *

 

Searching via gene name {#toc2}
-----------------------

Recently, you’ve learned about the protein ‘EPSIN1′ and you are curious
to know if there are any phosphorylation sites annotated for this
protein.

1.  Go to [Phospho.ELM](http://phospho.elm.eu.org) and enter protein
    name ‘epsin’ in the first form field.
    1.  You should see a table showing multiple hits in the database.
        Why?
    2.  Select ‘Epsin 1′. Now you’re at the results page. However, if
        you scroll down, you see results from multiple proteins. Why?
    3.  Which protein has the most annotation?
    4.  Go back to the Phospho.ELM startpage and query the database so
        that you’ll receive only results for this one protein.

2.  Start the Jalview Plugin and look at the conservation of the
    sequence (You’re looking for high conservation in non-structured
    regions).
    1.  Can you spot any?

* * * * *

 

Using BLAST to find homologous information {#toc3}
------------------------------------------

 

1.  Search for uniprot id ‘ABL1_MOUSE’
    1.  How many annotated phosphorylation sites do you find?

2.  Next, run
    [PhosphoBlast](http://phospho.elm.eu.org/pELMBlastSearch.html) on
    the
    [sequence](http://oz-masterclass.wikispaces.com/file/view/sequences_ELM.fasta/460946468/sequences_ELM.fasta)
    or ID of ‘ABL1_MOUSE’.
    1.  How many phosphorylation sites are found?
    2.  Why the difference?
    3.  In which proteins / organisms?

* * * * *

 

Comparing data from multiple sources: {#toc4}
-------------------------------------

 

1.  Go back to the phospho.elm startpage and search for uniprot id
    ‘EGFR_HUMAN’.
    1.  (Optional) There are quite a lot of annotations, several of
        which come from high-throughput sources which generally are of
        lower quality. Go back to the search form, tick the box ‘Do not
        show high throughput data’ and rerun the search again. You
        should see significantly fewer results.
    2.  Use the link at the top (‘EGFR’ or ‘P00533′) to go to Uniprot,
        scroll down (or click on ‘Subcellular location’) and try to get
        an idea of the protein topology in order to be able to answer
        the next question.
    3.  In which part of the protein do the most phosphorylation sites
        seem to be located?

2.  Now go to [PhosphoSitePlus](http://www.phosphosite.org) and search
    for ‘EGFR’, click ‘human’ and compare these results.
    1.  Scroll down to ‘Modification Sites and Domains’ to inspect the
        protein topology (might be useful to click at the link “Click
        here to view phosphorylation modifications only”)
    2.  Click the “Hide sites with only 1 MS/HTP reference” and “Show
        only sites with more than 5 references” buttons to get an idea
        for the confidence of these annotations
    3.  (Optional) PhosphoSitePlus allows you to compare phosphorylation
        side in different organisms side-by-side. Can you find an
        annotated phosphorylation site which is present in human, mouse,
        rat and pig? (It might help to click on “Show Multiple Sequence
        Alignment” to get a different overview) If you can find one,
        note down the position(s) and the residue, if you can’t find
        one, discuss with your neighbor why this could be.

Objective: Get familiar with the [ELM (Eukaryotic Linear Motif)](http://elm.eu.org) prediction tool . {#toc5}
=====================================================================================================

1.  Search protein SRC_HUMAN (accession P12931) for ELMs using the
    following parameters:
    -   Cell Compartment: **Not specified**
    -   Motif Probability Cutoff: **100**
    -   Taxonomic Context: (leave blank)

    1.  How many instances do you find (roughly)?

2.  Redo the search (again accession P12931) now using these parameters:
    -   Cell Compartment: **cytosol**
    -   Motif Probability Cutoff: **0.01**
    -   Taxonomic Context: Homo sapiens

    1.  How many instances do you find now?
    2.  How many of the instances are ‘annotated’?
    3.  Do the structural predictors/filters (SMART, GlobPlot, IUPRED,
        Secondary Structure) agree in terms of which regions are
        structured/disordered?
    4.  Compare the location of the annotated instances with structural
        information at hand (IUPRED, Secondary Structure).
    5.  (Optional) For the annotated instances, which of the ELM classes
        require a phosphorylation at a certain residue of the motif?
        (Hint: This information can be found in the description of the
        ELM class)
    6.  (Optional) Which residue in SRC_HUMAN corresponds to this and
        can you find evidence for a phosphorylation of this residue
        (using Phospho.ELM)?
    7.  Start the Jalview plugin to visualize the conservation of motifs
        in ‘SRC_HUMAN’.

3.  Submit the [sequence](http://uniprot.org/uniprot/P49023.fasta) of
    Paxillin (P49023) to ELM, using default parameters.
    1.  Compare the results with a search for the same sequence when
        using the cellular compartment ‘plasma membrane’
    2.  Remember the exercise from the Phospho.ELM section about
        Paxillin. Do you see why there where no phosphorylations
        annotated for the carboxy terminus of this protein?

4.  There are three annotated instances of the ELM class LIG_NRBOX in
    the protein NCOA2_HUMAN. Do they reside in ordered or disordered
    regions (according to IUPred and SMART)?
5.  Search ELM for the following proteins and familiarize yourself with
    the different modular organizations of the following proteins. You
    should focus on the different types of protein architectures, the
    different amount of information which is available from different
    resources as well as where functional motifs are located / in which
    part of the protein would you expect them? Feel free to click on the
    link to resources such as ‘Uniprot’ or ‘SMART’, to get more
    information about the selected protein.
    1.  EGFR_HUMAN
    2.  CASP9_HUMAN
    3.  EPN1_HUMAN
    4.  SMAD3_HUMAN
    5.  SOS1_HUMAN
    6.  PTN3_HUMAN
    7.  SRRM2_HUMAN
    8.  KMT2D_HUMAN
    9.  KI67_HUMAN
    10. AP180_HUMAN
    11. Q94833_TRIVA
    12. AMPH_HUMAN
    13. MAPK2_HUMAN
    14. CTNB1_HUMAN
    15. JUN_HUMAN

6.  Search elm.eu.org using the protein name ‘MDM4_HUMAN’ and look for
    the ‘USP binding motif’ DOC_USP7_1.
    1.  How many such motif instances are found in this protein
        sequence?
    2.  Try to assess the biological relevance of each of these
        instances.

7.  (Optional) Repeat this exercise with protein ‘AMPH_HUMAN’ and ELM
    class ‘LIG_Clathr_ClatBox_1′
    1.  (Optional) Again, try to assess the biological relevance of each
        of these instances. Is the annotation for the biological
        relevance in accordance with the globular structure?

8.  (Optional) You’re studying the cell surface expression of a receptor
    and find out that some isoforms are expressed at the surface
    (Q05586-2) while another isoform is retained in the endoplasmatic
    reticulum (Q05586-5). You want to investigate a possible role of
    linear motifs in this phenomenon.
    1.  First, align these sequences to see which parts are
        similar/identical and which are different (go to
        [http://www.uniprot.org/uniprot/Q05586](http://www.uniprot.org/uniprot/Q05586), 
        scroll down to ‘sequences’, add isoforms 2 and 5 to your
        basket, click your basket (top) and click on ‘align’).
    2.  Then use [http://elm.eu.org](http://elm.eu.org) to scan these
        sequences (one after the other, submit either ID or FASTA
        sequence) for linear motifs, using cell compartment filter
        ‘cytosol’. You’re looking for targeting motifs (TRG_\*).
    3.  By looking through the annotations of these targeting ELM
        classes, can you find motif instances that might be responsible
        for the different behaviour of the isoforms?
    4.  If there are multiple instances of that motif found per protein,
        can you use differential information (comparing the motifs found
        in the different isoforms) to narrow down the number of
        candidate instances?
    5.  Next, you sequence another isoform (Q05586-4) which also
        features this motif at a homologous position, but strangely does
        not get expressed at the cell surface. You discuss this with
        your colleague and he tells you that he recently found out that
        this protein also binds to the PDZ domain of DLG4. Can you come
        up with a hypothesis how this all fits together?

9.  (OPTIONAL) Search for linear motifs in the protein sequence
    SMAD3_HUMAN.
    1.  (OPTIONAL) Which annotated instances can you see?
    2.  (OPTIONAL) Click on one of the annotated docking motifs to read
        about a switching mechanism involving these motifs. How does
        this switch work?

10. (OPTIONAL) Caspase 9 is mainly globular protein. Focus on the
    carboxyterminal globular domain (CASc Caspase, interleukin-1 beta
    converting enzyme \# (ICE) homologues) and try to assess which
    modification sites (MOD_) are surface accessible (Hint: Mouse-over
    to find high accessibility scores with low p-values)

 

* * * * *

 

Objective: Get familiar with the [ELM](http://elm.eu.org) database . {#toc6}
====================================================================

Instances {#toc7}
---------

1.  (OPTIONAL) Search protein UNG_HUMAN (P13051) for annotated ELMs.
    1.  For the annotated instances, which of these ELM classes require
        a phosphorylation at a certain residue of the motif? (Hint: This
        information can be found in the description of the ELM class)
    2.  Which amino acid residue in UNG_HUMAN corresponds to this and
        can you find evidence for a phosphorylation of this residue
        (using Phospho.ELM)?

2.  (OPTIONAL) Get all annotated instances that contain the search term
    ”retinoblastoma” (again, using url
    [http://elm.eu.org/elms/browse_instances.html](http://elm.eu.org/elms/browse_instances.html)
    )
    1.  Compare the number of human instances with the number of viral
        instances.
    2.  Read the abstract for the ELM class LIG_Rb_LxCxE_1 to find
        out why so many viral proteins interact with Rb.

3.  (OPTIONAL) Search [Pubmed](http://www.ncbi.nlm.nih.gov/pubmed) for
    the terms “noonan syndrome” AND “motif” (you should get exactly one
    resulting publication, if not, make sure you use quotes around
    ‘”noonan syndrome”‘)
    1.  find the protein sequence that was analysed in this publication,
        retrieve the sequence from uniprot and submit it to ELM. Can you
        find the two mutation hotspots that are responsible for the
        syndrome described in the publication?

4.  (Optional) Get all annotated instances for ”Homo sapiens” that
    contain the search term ”ciliar” (Hint: Use
    [http://elm.eu.org/elms/browse_instances.html](http://elm.eu.org/elms/browse_instances.html)
    )
    1.  How many are there?
    2.  Which experimental evidence is annotated and how reliable is
        this evidence?
    3.  Try to get these instances as TSV-file (tab separated values)

 

* * * * *

 

Objective: Get familiar with the [Switches.ELM](http://switches.elm.eu.org) resource . {#toc8}
======================================================================================

 

1.  Enter “P53_HUMAN” in the box “Search database” and click submit.
    You should be presented a list of different motif switches annotated
    for this protein.
    1.  How many types of switches can you see? If you don’t know what a
        particular switch type or how it works, you can read up on it at
        the
        [Definitions](http://switches.elm.eu.org/index.php?page=definitions)
        page.
    2.  Click on the switch “P53_HUMAN DEG_MDM2″ at position 19-26.
    3.  In the visualisation on the right side, try to detect mutations
        that might affect this particular switch
    4.  Discuss with your neighbor how this switch works, how it’s
        triggered and what it’s outcome is…

2.  Click on the menu item “Analyse” and enter “BAD_HUMAN” in the
    search field, click on the entry and select residues GRSRSAPPNLW at
    position 95-105 and click “Submit”.\
     Compare the information/suggestions on the left with the
    visualization on the right and try to figure out what kind of motifs
    could be involved using which motifs?

* * * * *

References: {#toc8}
===========

- Alexander et al. Sci. Sig 2011 “Spatial exclusivity combined with positive and negative selection of phosphorylation motifs is the basis for context-dependent mitotic signaling” [URL](http://stke.sciencemag.org/cgi/content/short/4/179/ra42/DC1)
- Davey NE, Travé G and Gibson TJ (2011), *“How viruses hijack cell regulation”*, Trends Biochem Sci., Mar, 2011. Vol. 36, pp. 159-169. [DOI](http://dx.doi.org/10.1016/j.tibs.2010.10.002)
- Davey NE, Van Roey K, Weatheritt RJ, Toedt G, Uyar B, Altenberg B, Budd A, Diella F, Dinkel H and Gibson TJ (2012), *“Attributes of short linear motifs”*, Mol Biosyst., Jan, 2012. Vol. 8, pp. 268-281. [DOI](http://dx.doi.org/10.1039/c1mb05231d)
- Dinkel H, Michael S, Weatheritt RJ, Davey NE, Van Roey K, Altenberg B, Toedt G, Uyar B, Seiler M, Budd A, Jödicke L, Dammert MA, Schroeter C, Hammer M, Schmidt T, Jehl P, McGuigan C, Dymecka M, Chica C, Luck K, Via A, Chatr-Aryamontri A, Haslam N, Grebnev G, Edwards RJ, Steinmetz MO, Meiselbach H, Diella F and Gibson TJ (2012), *“ELM–the database of eukaryotic linear motifs”*, Nucleic Acids Res., Jan, 2012. Vol. 40, pp. D242-D251. [DOI](http://dx.doi.org/10.1093/nar/gkr1064)
- Dinkel H, Chica C, Via A, Gould CM, Jensen LJ, Gibson TJ and Diella F (2011), *“Phospho.ELM: a database of phosphorylation sites–update 2011.”*, Nucleic Acids Res., Jan, 2011. Vol. 39(Database issue), pp. D261-D267. [DOI](http://dx.doi.org/10.1093/nar/gkq1104)
- Dyson HJ and Wright PE (2005), *“Intrinsically unstructured proteins and their functions”*, Nat Rev Mol Cell Biol., Mar, 2005. Vol. 6, pp. 197-208. [DOI](http://dx.doi.org/10.1038/nrm1589)
- Van Roey K, Orchard S, Kerrien S, Dumousseau M, Ricard-Blum S, Hermjakob H and Gibson TJ (2013), *“Capturing cooperative interactions with the PSI-MI format”*, Database (Oxford). Vol. 2013, pp. bat066. [DOI](http://dx.doi.org/10.1093/database/bat066)
