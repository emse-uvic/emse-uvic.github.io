---
layout: default
---

<script type="text/javascript">
    function show_topic(topic) {
        topic_div = "#content-" + topic;
        content = $(topic_div).html();
        $('#topic-display').html(content);      
    }
</script>

<div class="pure-g" id="syllabus">
    <div class="sidebar pure-u-1 pure-u-md-1-5" id="syllabus-topics">
        <ul class="topics-list">
            <li><a id="topic-history" onclick="show_topic('history')" href="#"><span class="sidebar-link">History of Software Engineering</span></a></li>
            <li><a id="topic-empirical" onclick="show_topic('empirical')" href="#"><span class="sidebar-link">Empirical Software Engineering: Beliefs and Evidence</span></a></li>
            <li><a id="topic-design" onclick="show_topic('design')" href="#"><span class="sidebar-link">Design Science</span></a></li>
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
    <div class="hidden" id="content-history">
        <h3>Slides</h3>
        <iframe src="{{ "/assets/slides/week01-intro.pdf" | relative_url }}"></iframe>
        <h3>Optional Material</h3>
        <ul>
            <li>Chapter 1 of <a href="https://www.oreilly.com/library/view/software-engineering-at/9781492082781/">Software Engineering at Google</a> By Titus Winters, Tom Manshreck and Hyrum Wright, O'Reilly Media UVic link</li>
            <li><a href="https://www.microsoft.com/en-us/research/blog/exploding-software-engineering-myths/">Exploding Software Engineering Myths</a> by Janie Chang, Writer, Microsoft Research</li>
        </ul>
    </div>
    <div class="hidden" id="content-empirical">
        <div class="media">
            <h3>Media</h3>
            <iframe class="media-video" src="https://www.youtube.com/embed/Orghyn91ZMo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <br />
            <iframe class="media-podcast" src="https://anchor.fm/margaret-anne-d-storey/embed/episodes/Past--Present-and-Future-of-Empirical-Software-Engineering-A-QA-with-Greg-Wilson-eklhkc/a-a3f2kf5" frameborder="0" scrolling="no"></iframe>
            <br />
            <a href="{{ "/assets/slides/week02-empirical.pdf" | relative_url }}">Slides</a>
        </div>
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