---
layout: default
---

<script type="text/javascript">
    function show_topic(topic) {
        topic_div = "#content-" + topic;
        content = $(topic_div).html();
        $('#topic-display').html(content);      
    }

    $(document).ready(function() {
        show_topic('history');
    });
</script>

<div class="pure-g" id="syllabus">
    <div class="sidebar pure-u-1 pure-u-md-1-5" id="syllabus-topics">
        <ul class="topics-list">
            <li><a id="topic-history" onclick="show_topic('history')" href="#"><span class="sidebar-link">History of Software Engineering</span></a></li>
            <li><a id="topic-empirical" onclick="show_topic('empirical')" href="#"><span class="sidebar-link">Empirical Software Engineering: Beliefs and Evidence</span></a></li>
            <li><a id="topic-design" onclick="show_topic('design')" href="#"><span class="sidebar-link">Design Science</span></a></li>
            <li><a id="topic-methods" onclick="show_topic('methods')" href="#"><span class="sidebar-link">Research Methods in Software Engineering</span></a></li>
            <li><a id="topic-theory" onclick="show_topic('theory')" href="#"><span class="sidebar-link">Theories, Theoretical Frameworks, and Conceptual Frameworks</span></a></li>
            <li><a id="topic-literature" onclick="show_topic('literature')" href="#"><span class="sidebar-link">Literature Reviews for Software Engineering Research</span></a></li>
            <li><a id="topic-cse" onclick="show_topic('cse')" href="#"><span class="sidebar-link">Continuous Software Engineering</span></a></li>
            <li><a id="topic-review" onclick="show_topic('review')" href="#"><span class="sidebar-link">Code Review and Assessment</span></a></li>
            <li><a id="topic-diversity" onclick="show_topic('diversity')" href="#"><span class="sidebar-link">Diversity and Inclusion in Software Engineering</span></a></li>
            <li><a id="topic-collab" onclick="show_topic('collab')" href="#"><span class="sidebar-link">Collaboration, Communication, and Knowledge Flow</span></a></li>
            <li><a id="topic-productivity" onclick="show_topic('productivity')" href="#"><span class="sidebar-link">Developer and Team Productivity</span></a></li>
            <li><a id="topic-gaps" onclick="show_topic('gaps')" href="#"><span class="sidebar-link">Bridging Gaps</span></a></li>
        </ul>
    </div>
    <div class="topic-content pure-u-1 pure-u-md-4-5" id="topic-display">
    </div>
    <!--History-->
    <div class="hidden" id="content-history">
        <h2>History of Software Engineering</h2>
        <h3>Media</h3>
        <a href="{{ "/assets/slides/week01-intro.pdf" | relative_url }}">Lecture Slides</a>
        <h3>Optional Material</h3>
        <ul>
            <li>Chapter 1 of <a href="https://www.oreilly.com/library/view/software-engineering-at/9781492082781/">Software Engineering at Google</a> By Titus Winters, Tom Manshreck and Hyrum Wright, O'Reilly Media UVic link</li>
            <li><a href="https://www.microsoft.com/en-us/research/blog/exploding-software-engineering-myths/">Exploding Software Engineering Myths</a> by Janie Chang, Writer, Microsoft Research</li>
        </ul>
    </div>
    <!--Beliefs-->
    <div class="hidden" id="content-empirical">
        <h2>Empirical Software Engineering: Beliefs and Evidence</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/Orghyn91ZMo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Past--Present-and-Future-of-Empirical-Software-Engineering-A-QA-with-Greg-Wilson-eklhkc/a-a3f2kf5" frameborder="0" scrolling="no"></iframe>
            </div>
            <br />
            <a href="{{ "/assets/slides/week02-empirical.pdf" | relative_url }}">Lecture Slides</a>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://www.americanscientist.org/article/empirical-software-engineering">Empirical Software Engineering</a> by Greg Wilson, Jorge Aranda, American Scientist, Nov-Dec 2011.</li>
                <li><a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.121.3476&rep=rep1&type=pdf">The Princial Elements of the Nature of Science: Dispelling the Myths</a> by William F. McComas, 1998</li>
                <li><a href="http://chisel.cs.uvic.ca/pubs/storey-ESEM2017.pdf">Design Science Research in Software Engineering</a> by Storey, Enstrom, Host and Runeson, ESEM 2017</li>
                <li><a href="https://changelog.com/podcast/339">Why Engineers Write Bad Code</a> by Adam Barr (he explores the gap between industry and academia)</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://link.springer.com/book/10.1007/978-3-030-32489-6">Chapter 1, Contemporary Empirical Methods in Software Engineering</a>, Editors: Michael FeldererGuilherme Horta Travassos, Springer 2020</li>
                <li><a href="http://pages.cs.wisc.edu/~remzi/Naur.pdf">Programming as Theory Building</a> by Peter Naur, 1985.</li>
            </ul>
        </div>
    </div>
    <!--Design-->
    <div class="hidden" id="content-design">
        <h2>Design Science</h2>
        <div class="media">
            <h3>Media</h3>
            <a href="{{ "/assets/slides/week02-design.pdf" | relative_url }}">Lecture Slides</a>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="http://chisel.cs.uvic.ca/pubs/storey-ESEM2017.pdf">Design Science Research in Software Engineering</a> by Storey, Enstrom, Host and Runeson, ESEM 2017.</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="http://chisel.cs.uvic.ca/pubs/storey-ESEM2017.pdf">Using a Visual Abstract as a Lens for Communicating and Promoting Design Science Research in Software Engineering</a> by Storey, Engstrom, Host, Runeson and Bjarnason, ESEM, 2017.</li>
                <li><a href="https://link.springer.com/article/10.1007%2Fs10664-020-09818-7">How software engineering research aligns with design science: a review</a> by Emelie Engström, Margaret-Anne Storey, Per Runeson, Martin Höst & Maria Teresa Baldassarre, Empirical Software Engineering, volume 25, pages 2630–2660, 2020.</li>
                <li><a href="https://link.springer.com/chapter/10.1007%2F978-3-642-33371-2_3?LI=true">Design Science Research as Movement Between Individual and Generic Situation-Problem–Solution Spaces</a>, by Ilia Bider, Paul Johannesson and Erik Perjons, Designing Organizational Systems. Lecture Notes in Information Systems and Organisation, vol 1. Springer, Berlin, Heidelberg. 2012.</li>
                <li><a href="https://t.co/XopxZWE3Xo?amp=1">10 min introduction</a> by Runeson, Engstrom, Storey</li>
            </ul>
        </div>
    </div>
    <!--Research Methods-->
    <div class="hidden" id="content-methods">
        <h2>Research Methods in Software Engineering</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry  media-entry-left">
                <iframe src="https://www.youtube.com/embed/z-Yr27qtePM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Grounded-Theory-in-Software-Engineering-A-Talk-and-QA-with-Rashina-Hoda-el5kjj/a-a3ifh82" frameborder="0" scrolling="no"></iframe>
            </div>
            <br />
            <a href="{{ "/assets/slides/week03-methods.pdf" | relative_url }}">Lecture Slides</a>
            <br />
            <a href="{{ "/assets/slides/week03-guest.pdf" | relative_url }}">Guest Speaker Slides</a>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="http://www.cs.utoronto.ca/~sme/papers/2007/SelectingEmpiricalMethods.pdf">Selecting a research method</a> by Easterbrook et al.</li>
                <li><a href="https://link.springer.com/article/10.1007/s10664-011-9161-0">Developing a grounded theory to explain the practices of self-organizing Agile teams</a> by <a href="https://research.monash.edu/en/persons/rashina-hoda">Hoda, Rashina</a> & Noble, James & Marshall, Stuart. (2012). Empirical Software Engineering - ESE. 17. 1-31.</li>
                <li><a href="https://www.sciencedirect.com/science/article/pii/B9780080515748500194">Methodology Matters</a> by McGrath</li>
                <li><a href="https://medium.com/bits-and-behavior/grand-challenges-in-program-comprehension-and-software-repository-mining-my-keynote-on-7bf2cfc182a5">Challenges in Program Comprehension and Software Repository Mining</a>, Talk by Amy Ko (Video)</li>
                <li><a href="https://dl.acm.org/doi/10.1145/2597073.2597074">The promises and perils of mining GitHub</a> by Eirini Kalliamvakou, Georgios Gousios, Kelly Blincoe, Leif Singer Daniel M Germán, Daniela E Damian, MSR 2014</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li>General Resources</li>
                <ul>
                    <li><a href="https://www.elsevier.com/books/research-methods-in-human-computer-interaction/lazar/978-0-12-805390-4">Research Methods in Human-Computer Interaction, 2nd Edition</a> by Paul Lazar, Elsevier, 2017.</li>
                    <li><a href="https://www.cambridge.org/core/books/research-methods-for-humancomputer-interaction/43E95E979117C42DF822673D098474D2">Research Methods for Human-Computer Interaction</a> Edited by Paul Cairns and Anna Cox, Cambridge University Press, 2008.</li>
                    <li><a href="https://ieeexplore.ieee.org/document/799955">Qualitative methods in empirical studies of software engineering</a> by C. B. Seaman, IEEE Transactions on Software Engineering, vol. 25, no. 4, pp. 557-572, July-Aug. 1999.</li>
                    <li><a href="https://us.sagepub.com/en-us/nam/research-design/book255675">Research design: Qualitative, quantitative, and mixed methods approaches</a>, Creswell & Creswell. Sage publications, 5th edition.</li>
                    <li><a href="https://github.com/acmsigsoft/EmpiricalStandards/blob/master/Empirical%20Standards.pdf">ACM SIGSOFT Empirical Standards</a> By Paul Ralph et al., 2020.</li>
                    <li><a href="https://www.researchgate.net/publication/326540762_The_ABC_of_Software_Engineering_Research">The ABC of Software Engineering Research</a> by Stol and Fitzgerald, TOSEM 2018.</li>
                    <li><a href="The Research Onion">The Research Onion</a></li>
                </ul>
                <li>Data Science and Mining Repositories</li>
                <ul>
                    <li><a href="https://www.elsevier.com/books/perspectives-on-data-science-for-software-engineering/menzies/978-0-12-804206-9?countrycode=US&format=print&utm_source=google_ads&utm_medium=paid_search&utm_campaign=canadashopping&gclid=CjwKCAjwkoz7BRBPEiwAeKw3q6IdWnBmgg4ZFIMpU6XMzITW4PFErv6VHHEqJ29NflbtSsG6WIFv5xoCrEIQAvD_BwE&gclsrc=aw.ds">Perspectives on Data Science for Software Engineering, 1st Edition</a>, Editors: Tim Menzies Laurie Williams Thomas Zimmerman, Morgan Kaufmann, 2016.</li>
                </ul>
                <li>Analyzing and Interpreting Data</li>
                <ul>
                    <li><a href="https://www.researchgate.net/publication/263088251_Grounded_Theory_for_Geeks">Grounded theory for Geeks</a> by Rashina Hoda, James Noble, Stuart Marshall. ACM International Conference Proceeding Series. 2011.</li>
                    <li><a href="https://uk.sagepub.com/en-gb/eur/constructing-grounded-theory/book235960">Constructing Grounded Theory, SECOND EDITION</a>, by Kathy Charmaz, Sage Publishing 2014.</li>
                    <li><a href="https://pubmed.ncbi.nlm.nih.gov/27580703/">Beyond a good story: from Hawthorne Effect to reactivity in health professions education research</a> by Elise Paradis and Gary Sutkin Med Educ. 2017 Jan;51(1):31-39. doi: 10.1111/medu.13122. Epub 2016 Aug 31.</li>
                    <li><a href="https://us.sagepub.com/en-us/nam/qualitative-data-analysis/book246128">Qualitative data analysis: A methods sourcebook</a> by Miles, Matthew B., A. Michael Huberman, and Johnny Saldana. 2014. 4th edition.</li>
                    <li><a href="https://www.cambridge.org/core/books/doing-better-statistics-in-humancomputer-interaction/1D19B5419225C05D6E4FE189A345BDB8">Doing Better Statistics in Human-Computer Interaction</a>, by Paul Cairns, 2019.</li>
                    <li><a href="https://www.youtube.com/watch?v=gn7Pr8M_Gu8)by">Grounded Theory - Open Coding</a> by Graham R Gibbs 2010, posted on YouTube.</li>
                </ul>
                <li>Case Study Research</li>
                <ul>
                    <li><a href="https://link.springer.com/article/10.1007%2Fs10664-008-9102-8">Guidelines for conducting and reporting case study research in software engineering</a> by Per Runeson and Martin Höst, Empirical Software Engineering 14, 131 (2009).</li>
                </ul>
                <li>Survey Research</li>
                <ul>
                    <li><a href="https://www.slideshare.net/mendezfe/surveys-in-software-engineering">Tutorial on Surveys in Software Engineering</a></li>
                    <li><a href="https://www.semanticscholar.org/paper/Sampling-in-Software-Engineering-Research%3A-A-Review-Baltes-Ralph/8587736a41c9f22a432074e6344a1c9998ae7338">Sampling in Software Engineering Research: A Critical Review and Guidelines</a> by Baltes and Ralph, 2020.</li>
                </ul>
                <li>Ethnography</li>
                <ul>
                    <li><a href="http://oro.open.ac.uk/45166/">The Role of Ethnographic Studies in Empirical Software Engineering</a>, by Helen Sharp et al., IEEE Transactions on Software Engineering, 42(8) pp. 786–804, 2016.</li>
                    <li><a href="https://dl.acm.org/doi/abs/10.1109/ICSE.2007.87">The Social Dynamics of Pair Programming</a> by Jan Chong and Tom Hurlbutt, ICSE '07: Proceedings of the 29th international conference on Software EngineeringMay 2007 Pages 354–363. (Nice example of ethnography)</li>
                </ul>
                <li>Action Research</li>
                <ul>
                    <li><a href="https://link.springer.com/chapter/10.1007/978-3-030-10801-4_4">Action Research in Software Engineering</a></li>
                </ul>
                <li>Experiments</li>
                <ul>
                    <li><a href="https://www.springer.com/gp/book/9783642290435">Experimentation in Software Engineering</a> by Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A., Springer 2012.</li>
                </ul>
                <li>Mixed Methods</li>
                <ul>
                    <li><a href="https://ieeexplore.ieee.org/document/7965402">Combining Quantitative and Qualitative Studies in Empirical Software Engineering Research</a> by Massimiliano Di Penta and Damian Andrew Tamburri, ICSE Companion, 2017.</li>
                    <li>Creswell book, referenced above.</li>
                </ul>
                <li>Validity and Research Limitations</li>
                <ul>
                    <li><a href="https://psycnet.apa.org/record/2017-12051-001">A total quality framework approach to sharing qualitative research data: Comment on Dubois et al.</a> Roller, M. R., & Lavrakas, P. J. (2018). Qualitative Psychology, 5(3), 394–401</li>
                    <li><a href="https://link.springer.com/article/10.1007/s11135-006-9000-3#citeas">Validity and Qualitative Research: An Oxymoron?</a> by Onwuegbuzie, A.J., Leech, N.L. Qual Quant 41, 233–249 (2007).</li>
                    <li>See also the Creswell <&amp;> Creswell book referenced above.</li>
                </ul>
            </ul>
        </div>
    </div>
    <!--Theory-->
    <div class="hidden" id="content-theory">
        <h2>Theories, Theoretical Frameworks, and Conceptual Frameworks</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry  media-entry-left">
                <iframe src="https://www.youtube.com/embed/_8aPAGD6tdA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Theories--Theoretical-Frameworks-in-Software-Engineering-A-Talk-and-QA-with-Elise-Paradis-el5kri/a-a3ifijb" frameborder="0" scrolling="no"></iframe>
            </div>
            <br />
            <a href="{{ "/assets/slides/week04-theory.pdf" | relative_url }}">Lecture Slides</a>
            <br />
            <a href="{{ "/assets/slides/week04-guest.pdf" | relative_url }}">Guest Speaker Slides</a>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://link.springer.com/chapter/10.1007/978-1-84800-044-5_12">Building Theories in Software Engineering</a> by Dag I. K. Sjøberg, Tore Dybå, Bente C. D. Anda, Jo E. Hannay, Guide to Advanced Empirical Software Engineering pp 312-336, Spring 2008.</li>
                <li><a href="https://www.researchgate.net/profile/Harasit_Paul4/post/what_is_the_difference_between_theoretical_framework_and_conceptual_framework/attachment/5ed558e7152fe900010c39cc/AS%3A897701948448768%401591040231038/download/varpio2019.pdf">The Distinctions Between Theory, Theoretical Framework, and Conceptual Framework</a> by Lara Varpio, <a href="https://www.whatiscollaboration.org/">Elise Paradis</a>, Sebastian Uijtdehaage, Meredith Young, Academic Medicine: Journal of the Association of American Medical Colleges, 2019.</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://www.sciencedirect.com/science/article/pii/S0167642314005425">Theory-oriented software engineering</a> by Klas-Jan Stol and Brian Fitzgerald, Science of Computer Programming, Volume 101, 1 April 2015, Pages 79-98.</li>
            </ul>
        </div>
    </div>
    <!--Literature-->
    <div class="hidden" id="content-literature">
        <h2>Literature Reviews for Software Engineering Research</h2>
        <div class="media">
            <h3>Media</h3>
            <a href="{{ "/assets/slides/week05-litrev.pdf" | relative_url }}">Lecture Slides</a>
            <br />
            <a href="{{ "/assets/slides/week05-wwh.pdf" | relative_url }}">The Who, What, How Framework and Design Science Revisited</a>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="http://robertfeldt.net/publications/petersen_ease08_sysmap_studies_in_se.pdf">Systematic Mapping Studies in Software Engineering</a>, by Petersen et al., EASE 2008.</li>
                <li><a href="https://link.springer.com/article/10.1007%2Fs10664-020-09858-z">The who, what, how of software engineering research: a socio-technical framework</a> by Storey, M., Ernst, N.A., Williams, C. et al. Empir Software Eng 25, 4097–4129 (2020).</li>
                <li><a href="https://link.springer.com/article/10.1007/s10664-020-09818-7">How software engineering research aligns with design science: a review</a> by Emelie Engström, Margaret-Anne Storey, Per Runeson, Martin Höst & Maria Teresa Baldassarre, Empirical Software Engineering volume 25, pages 2630–2660, 2020.</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li>Literature review related papers</li>
                <ul>
                    <li><a href="https://link.springer.com/chapter/10.1007/978-3-030-32489-6_14">Benefitting from the Grey Literature in Software Engineering Research</a> by Vahid Garousi, Michael FeldererMika V. Mäntylä, Austen Rainer, Contemporary Empirical Methods in Software Engineering pp 385-413, 2020.</li>
                    <li><a href="https://www.elsevier.com/__data/promis_misc/525444systematicreviewsguide.pdf">Guidelines for performing Systematic Literature Reviews in Software Engineering</a>, Version 2.3, EBSE Technical Report 2007, Software Engineering Group, School of Computer Science and Mathematics, Keele University.</li>
                    <li><a href="https://www.sciencedirect.com/science/article/pii/S0950584913001560?casa_token=DmP0XP_UAfwAAAAA:hy0GIIiSF463LBaBJclDbON6O8_ZziC0vBjjh3fSk5ANIts9n27pqlwRF1EBMYveKKX7uVn5">A systematic review of systematic review process research in software engineering</a> by Barbara Kitchenham and Pearl Brereton, Information and Software Technology, Volume 55, Issue 12, December 2013, Pages 2049-2075.</li>
                    <li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0950584910000467">Systematic literature reviews in software engineering – A tertiary study</a> by Barbara Kitchenham et al., Information and Software Technology, Volume 52, Issue 8, August 2010, Pages 792-805.</li>
                    <li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0950584915000646?casa_token=1NlNiXiuApIAAAAA:b-fpb6OC_wS53TAxSfrd3FN389IhBiUb1nyjtgooz4V0tqqO9hJVPjmBYuRaXJOXqbP9Kgn0">Guidelines for conducting systematic mapping studies in software engineering: An update</a>, by Kai Petersen, Sairam Vakkalanka, Ludwik Kuzniarz, Information and Software Technology, Volume 64, 2015.</li>
                    <li><a href="https://research-seminar.github.io/slides/EiriniKalliamvakou_SystematicLiteratureReviews.pdf">A Guide to SLRs in Software Engineering</a> presented by Eirini Kalliamvakou, University of Victoria.</li>
                </ul>
                <li>Example literature reviews in software engineering (related to Activity)</li>
                <ul>
                    <li><a href="https://portal.research.lu.se/portal/files/4288476/3738217.pdf">A systematic review on regression test selection techniques</a> by Engstrom et al., IST 2010.</li>
                    <li><a href="https://www.researchgate.net/publication/260734375_Motivation_in_software_engineering_A_systematic_review_update">Motivation in Software_engineering: A_systematic review update</a> by Beecham et al., IST 2008.</li>
                    <li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0164121215000989">Behavioral software engineering: A definition and systematic literature review</a> by Per Lenberg et al., JSS 2015.</li>
                    <li><a href="https://alexeyza.com/pdf/botse2019invited.pdf">Defining and Classifying Software Bots: A Faceted Taxonomy</a> by Lebeuf et al., ICSE/BotSE 2019.</li>
                </ul>
            </ul>
        </div>
    </div>
    <!--Continuous-->
    <div class="hidden" id="content-cse">
        <h2>Continuous Software Engineering</h2>
        <div class="media">
            <h3 class="pure-u-1-1">Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/S6USW-ee_u0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Devops-and-High-Performing-Teams-A-QA-with-Nicole-Forsgren--GitHub-ele7tb/a-a3kb9go" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/UHMLMi_Ks8o" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/AIOps-in-Continuous-Software-Engineering-A-QA-with-Chandra-Maddila-elaru2/a-a3jgjv8" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/VtVl30k3xuQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Ethnographic-Studies-of-Work-Practices-in-SE-A-QA-with-Eben-Haber-elbm3b/a-a3jnp02" frameborder="0" scrolling="no"></iframe>
            </div>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://www.agilealliance.org/resources/videos/continuously-deploying-security-laurie-williams-xp-2018/">Continuously Deploying Security</a> by Laurie Williams, 2018.</li>
                <li><a href="https://www.microsoft.com/en-us/research/lab/microsoft-research-india/articles/podcast-can-we-make-better-software-by-using-ml-and-ai-techniques-with-chandra-madilla-and-chetan-bansal/">Can we make better software by using ML and AI techniques?</a> With Chandra Maddila and Chetan Bansal, August 2020.</li>
                <li><a href="https://oxford-universitypressscholarship-com.ezproxy.library.uvic.ca/view/10.1093/acprof:oso/9780195374124.001.0001/acprof-9780195374124-chapter-2">Chapter 2 of Taming Information Technology: Lessons from Studies of System Administrators</a>, by Eser Kandogan, Paul P. Maglio, Eben M. Haber and John Bailey, Oxford Press, 2012.</li>
                <li><a href="https://www.youtube.com/watch?v=RBuPlMTXuFc">The Key to High Performance: What the Data Says</a> by Nicole Forsgren, GitHub OR you may instead want to listen to this Podcast: <a href="https://a16z.com/2018/03/28/devops-org-change-software-performance/">Feedback Loops — Company Culture, Change, and DevOps</a> by Nicole Forsgren, Jez Humble, and Sonal Chokshi</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://www.brian-fitzgerald.com/wp-content/uploads/2019/02/The-Journal-of-Systems-and-Software-2015-Continuous-software-engineering-A-roadmap-and-agenda.pdf">Continuous software engineering: A roadmap and agenda</a> by Brian Fitzgerald and Klaas-Jan Stol, JSS 2015.</li>
                <li><a href="https://nicolefv.com/book">Accelerate: Building and Scaling High Performing Technology Organizations</a> by Nicole Forsgren, Jez Humble, and Gene Kim, 2018.</li>
                <li><a href="https://oxford.universitypressscholarship.com/view/10.1093/acprof:oso/9780195374124.001.0001/acprof-9780195374124">Taming Information Technology: Lessons from Studies of System Administrators</a> by Eser Kandogan, Paul Maglio, Eben Haber, and John Bailey, Oxford University Press, 2012.</li>
            </ul>
        </div>
    </div>
    <!--Review-->
    <div class="hidden" id="content-review">
        <h2>Code Review and Assessment</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/Lo5cNcjdrmM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Empirical-Studies-of-Code-Review-Practices-and-Tools-and-What-Lies-Ahead-A-QA-with-Christian-Bird-elnipv/a-a3mdaju" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry  media-entry-right">
                <iframe src="https://www.youtube.com/embed/eriNYdKHeNc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/The-Code-Review-Experience-in-Azure--Microsoft-A-Presentation-and-QA-with-Brian-Houck--Microsoft-elofve/a-a3mh633" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry  media-entry-left">
                <iframe src="https://www.youtube.com/embed/E-6qDKUBa1s" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/How-Test-Assertions-are-Correlated-with-Test-Suite-Effectiveness-A-QA-with-Ali-Mesbah-ellgtd/a-a3luas1" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/MWeCMjtYdIs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Revisiting-the-iconic-Secret-Life-of-Bugs-paper-A-QA-with-Jorge-Aranda-elm8fb/a-a3m3kgu" frameborder="0" scrolling="no"></iframe>
            </div>
        </div>
        <div class="material">
            <h3 class="">Assigned Material</h3>
            <ul class="">
                <li><a href="http://ece.ubc.ca/~amesbah/resources/papers/fse15.pdf">Assertions Are Strongly Correlated with Test Suite Effectiveness</a> by Yucheng Zhang and Ali Mesbah, ESEC/FSE 2015.</li>
                <li><a href="https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/secret.pdf">The Secret Life of Bugs: Going Past the Errors and Omissions in Software Repositories</a>, by Jorge Aranda and Gina Venolia, ICSE '09: Proceedings of the 31st International Conference on Software Engineering, May 2009, Pages 298–308.</li>
                <li><a href="https://www.microsoft.com/en-us/research/publication/expectations-outcomes-and-challenges-of-modern-code-review/">Expectations, Outcomes, and Challenges of Modern Code Review</a> by Christian Bird Alberto Bacchelli, ICSE 2013.</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://refactoring.com/">Refactoring Book</a></li>
                <li><a href="http://cabird.com/pubs/macleod2017codereviewing.pdf">Code Reviewing in the Trenches: Understanding Challenges and Best Practices</a> by Laura MacLeod, M. Greiler, M. Storey, C. Bird and J. Czerwonka, IEEE Softwre 2017.</li>
            </ul>
        </div>
    </div>
    <!--Diversity-->
    <div class="hidden" id="content-diversity">
        <h2>Diversity and Inclusion in Software Engineering</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/-cDNfAqzY3Y" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Lessons-learned-from-an-Autism-Coding-Camp-A-QA-with-Andrew-Begel-and-Paige-Rodeghero-eo5ppn/a-a46sikj" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/Ug9KbyuIHjE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Diversity-in-Software-Engineering-A-QA-with-Alexander-Serebrenik-em8lqp/a-a3q1mql" frameborder="0" scrolling="no"></iframe>
            </div>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://cbsoft2020.imd.ufrn.br/palestrante.php?id=alexander">Gender in Open-Source Software Development</a> by Alexander Serebrenik, CBSoft 2020, Brazil</li>
                <li><a href="https://peerj.com/articles/cs-111/">Gender differences and bias in open source: pull request acceptance of women versus men</a> by Josh Terrell, Andrew Kofink, Justin Middleton, Clarissa Rainear, Emerson Murphy-Hill, Chris Parnin, Jon Stallings, May 2017, PeerJ.</li>
                <li><a href="https://github.com/margaretstorey/EmseUvic2020/blob/master/references/BegelAutismCodingCamp.pdf">Autism Coding Camp</a> by Andrew Begel et al., SIGCSE 2020</li>
                <li><a href="https://www.youtube.com/watch?v=tgSn-Ao0VTk">Gender Inclusivity Software Engineering</a> by Margaret Burnett and Anita Sarma</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="http://web.engr.oregonstate.edu/~sarmaa/wp-content/uploads/2020/08/icse20-genderMag-practices.pdf">Engineering Gender-Inclusivity into Software: Ten Teams’ Tales from the Trenches</a> by C. Hilderbrand, C. Perdriau, L. Letaw, J. Emard, Z. Steine-Hanson, M. Burnett, and A. Sarma, , ACM/IEEE 42nd International Conference on Software Engineering (ICSE), May 2020.</li>
                <li><a href="https://www.youtube.com/watch?v=a7tt18Gh8M0&feature=emb_logo">Is 40 the new 60?</a> by Alexander Serebrenik</li>
                <li><a href="https://www.youtube.com/watch?v=yP028rbR_t4">Golden Rules of Building Communities</a> by Denae Ford Robinson, OCTO Speaker Series, 2020.</li>
            </ul>
        </div>
    </div>
    <!--Collaboration-->
    <div class="hidden" id="content-collab">
        <h2>Collaboration, Communication, and Knowledge Flow</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/vE0Gde0RuKQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Role-of-identity--social-norms-in-building-sustainable-online-communities-A-QA-with-Anna-Filipova-emlutn/a-a3sq8f1" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/eTfKt64oCK4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Social-Technical-Coordination-in-Software-Engineering-A-QA-with-Jim-Herbsleb-emp3op/a-a3tectu" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/E9p88Ut0jlI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/How-war-stories-can-reveal-what-really-happens-in-software-engineering--A-QA-with-Carolyn-Seaman-emjt2h/a-a3sdun7" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/beddlJwfkoA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                No Podcast Version Available.
            </div>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://userpages.umbc.edu/~cseaman/papers/ISTJ07.pdf">Revealing actual documentation usage in software maintenance through war stories</a> by Wayne Lutters and Carolyn Seaman, IST 2007.</li>
                <li><a href="https://collabtech2020.colaps.ut.ee/keynote/">The role of identity and social norms in building sustainable online communities and successful remote teams</a> by Anna Filippova, GitHub</li>
                <li><a href="https://youtu.be/v0CSnYvd0C4?t=1769">Socio-Technical Coordination</a> by Jim Herbsleb, ICSE 2014</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://www.researchgate.net/publication/44279493_The_Social_Identity_Perspective">The Social Identity Perspective: Intergroup Relations, Self-Conception, and Small Groups</a>, by Michael A. Hogg, Dominic Abrams, Sabine Otten, Steve Hinkle, Small Group Research. 2004; 35(3):246-276.</li>
                <li><a href="https://dl.acm.org/doi/pdf/10.1145/2950290.2994160?casa_token=WgwFs4AVPYcAAAAA:U8GMwVuZsq6KIsN9ExDs4VKkvGRUk2FHG7D_qFpQdnobhHDerYaxu42AcJZrr1CMCoiTUoY3zY_RIw">Building a socio-technical theory of coordination: why and how (outstanding research award)</a> by James Herbsleb, FSE 2016.</li>
                <li><a href="https://drive.google.com/file/d/1ZcPgU5q71A9_NkyRCUCRsUrppzctCiGY/view">Observation as a Data Collection Technique for Software Engineering Research</a> by Carolyn Seaman, IASESE 2019 Tutorial.</li>
                <li><a href="https://cs.adelaide.edu.au/~christoph/CBSoftTutorial.pdf">A Tutorial on Qualitative Data Coding when Mining Software Repositories</a> by Christoph Treude.</li>
            </ul>
        </div>
    </div>
    <!--Productivity-->
    <div class="hidden" id="content-productivity">
        <h2>Developer and Team Productivity</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/hA4QbkraKn4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/The-Many-Faces-of-Software-Developer-Productivity-A-QA-with-Tom-ZimmermannDr--Tom-Zimmermann-visits-our-course-on-empirical-software-engineering-and-discusses-his-many-years-of-research-on-developer-en0hhh/a-a3v218s" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/CyTgqtw2PhU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Experiences-of-Software-Developers-Working-from-Home-During-the-Pandemic-A-QA-with-Jenna-Butler-enjfas/a-a433q9t" frameborder="0" scrolling="no"></iframe>
            </div>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://blubrry.com/microsoftresearch/53765597/077r-the-productive-software-engineer-with-dr-tom-zimmermann/">The productive software engineer</a> with Dr. Tom Zimmermann</li>
                <li><a href="https://www.youtube.com/watch?v=OFKv8vVQeZM">Improving Engineering Productivity at Scale</a> by Ciera Jaspan, SPLASH 2019 (Video) OR <a href="https://softwareengineeringdaily.com/2019/05/22/monolithic-repositories-with-ciera-jaspan/">Monolithic Repositories</a> with Ciera Jaspan</li>
                <li><a href="https://www.microsoft.com/en-us/research/publication/challenges-and-gratitude-a-diary-study-of-software-engineers-working-from-home-during-covid-19-pandemic/">Challenges and Gratitude: A Diary Study of Software Engineers Working From Home During Covid-19 Pandemic</a> by Jenna Butler, Microsoft </li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://arxiv.org/abs/2008.11147">A Tale of Two Cities: Software Developers Working from Home During the COVID-19 Pandemic</a> by Denae Ford, Margaret-Anne Storey, Thomas Zimmermann, Christian Bird, Sonia Jaffe, Chandra Maddila, Jenna L. Butler, Brian Houck, Nachiappan Nagappan</li>
                <li><a href="https://conf.researchr.org/details/icse-2020/icse-2020-Journal-First/49/Towards-a-theory-of-software-developer-job-satisfaction-and-perceived-productivity">Towards a theory of software developer job satisfaction and perceived productivity</a> by Margaret-Anne Storey, Thomas Zimmermann, Christian Bird, Jacek Czerwonka, Brendan Murphy, Eirini Kalliamvakou, TSE journal paper presented at ICSE 2020.</li>
                <li><a href="https://research.google/pubs/pub47853/">What Predicts Software Developers’ Productivity?</a> by Emerson Murphy-Hill Ciera Jaspan Caitlin Sadowski David C. Shepherd Michael Phillips Collin Winter Andrea Knight Dolan Edward K. Smith Matthew A. Jorde, Transactions on Software Engineering (2019).</li>
                <li><a href="https://research.google/pubs/pub49446/">Enabling the Study of Software Development Behavior with Cross-Tool Logs</a> by Ciera Jaspan Matthew Jorde Carolyn Denomme Egelman Collin Green Ben Holtz Edward K. Smith Maggie Morrow Hodges Andrea Marie Knight Dolan Elizabeth Kammer Jillian Dicker Caitlin Harrison Sadowski James Lin Lan Cheng Mark Canning Emerson Murphy-Hill, IEEE Software, vol. Special Issue on Behavioral Science of Software Engineering (2020).</li>
            </ul>
        </div>
    </div>
    <!--Gaps-->
    <div class="hidden" id="content-gaps">
        <h2>Bridging Gaps</h2>
        <div class="media">
            <h3>Media</h3>
            <div class="media-entry media-entry-left">
                <iframe src="https://www.youtube.com/embed/jMeNUbtgWE4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Promoting-Human-Flourishing-Through-Ethical-Software-Development--A-Talk-and-QA-with-Michael-Hilton-enkkav/a-a43bjle" frameborder="0" scrolling="no"></iframe>
                <br />
                <a href="https://drive.google.com/file/d/1pRa1mZm3PgHbhMJg0LgG8FQ6gHqSsLLm/view">Promoting Human Flourishing through Ethical Software Developmen</a>t by Michael Hilton
            </div>
            <div class="media-entry media-entry-right">
                <iframe src="https://www.youtube.com/embed/mP3nb9O_yyU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <br />
                <iframe src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/The-fairness-of-peer-review-and-insights-from-studies-of-open-source-A-QA-with-Daniel-German-enl9mt/a-a43ghp9" frameborder="0" scrolling="no"></iframe>
            </div>
            <div class="media-entry media-entry-left">
                No Video Available.
                <br />
                No Podcast Available.
                <br />
                <a href="{{ "/assets/slides/workshop06_czerwonka.pdf" | relative_url }}">Bridging Gaps between Research and Industry in Software Engineering</a> by Jacek Czerwonka, Microsoft.
            </div>
        </div>
        <div class="material">
            <h3>Assigned Material</h3>
            <ul>
                <li><a href="https://www.researchgate.net/publication/327561403_Was_My_Contribution_Fairly_Reviewed_A_Framework_to_Study_the_Perception_of_Fairness_in_Modern_Code_Reviews">"Was My Contribution Fairly Reviewed?" A Framework to Study the Perception of Fairness in Modern Code Reviews</a> by Daniel German et al. ICSE 2018 OR <a href="https://www2.slideshare.net/dmgerman/fairness-and-code-reviews">Was my contribution reviewed fairly?</a> by Daniel German</li>
                <li><a href="https://www.microsoft.com/en-us/research/wp-content/uploads/2015/05/PID3556473.pdf">Code Reviews Do Not Find Bugs: How the Current Code Review Best Practice Slows Us Down</a> by Jacek Czerwonka, Michaela Greiler, and Jack Tilford, ICSE 2015</li>
            </ul>
            <h3>Optional Material</h3>
            <ul>
                <li><a href="https://speakerdeck.com/michaelhilton/promoting-human-flourishing-through-ethical-software-development">Promoting Human Flourishing Through Ethical Software Development</a> by Michael Hilton</li>
                <li><a href="https://dl.acm.org/doi/10.1145/2597073.2597074">The promises and perils of mining GitHub</a> by Eirini Kalliamvakou, Georgios Gousios, Kelly Blincoe, Leif Singer Daniel M Germán, Daniela E Damian, MSR 2014</li>
            </ul>
        </div>
    </div>
</div>