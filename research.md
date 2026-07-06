---
layout: page
permalink: /research/
title: Research
---

<style>
  .research-intro {
    font-size: 1.05rem;
    line-height: 1.7;
    margin-bottom: 1.75rem;
  }

  .research-note {
    background: #f7f7f7;
    border-left: 4px solid #555;
    padding: 1rem 1.1rem;
    margin: 1.5rem 0;
    border-radius: 6px;
    line-height: 1.6;
  }

  .theme-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
    gap: 1rem;
    margin: 1.5rem 0 2.25rem 0;
  }

  .theme-card {
    border: 1px solid #e5e5e5;
    border-radius: 12px;
    padding: 1rem;
    background: #fff;
  }

  .theme-card h3 {
    margin-top: 0;
    margin-bottom: 0.45rem;
    font-size: 1.05rem;
  }

  .theme-card p {
    margin: 0;
    line-height: 1.55;
    font-size: 0.95rem;
  }

  .research-line {
    border: 1px solid #e6e6e6;
    border-radius: 16px;
    padding: 1.25rem;
    margin: 2rem 0;
    background: #fff;
  }

  .research-line h2 {
    margin-top: 0;
  }

  .research-line-layout {
    display: grid;
    grid-template-columns: minmax(0, 1.55fr) minmax(260px, 0.9fr);
    gap: 1.25rem;
    align-items: start;
  }

  @media (max-width: 800px) {
    .research-line-layout {
      grid-template-columns: 1fr;
    }
  }

  .research-visual {
    border: 1px dashed #b8b8b8;
    border-radius: 14px;
    min-height: 260px;
    padding: 1rem;
    background:
      linear-gradient(135deg, rgba(0,0,0,0.025), rgba(0,0,0,0.055));
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    overflow: hidden;
  }

  .research-visual img {
    width: 100%;
    height: auto;
    border-radius: 12px;
    display: block;
    margin-bottom: 0.75rem;
  }

  .placeholder-label {
    text-transform: uppercase;
    letter-spacing: 0.08em;
    font-size: 0.75rem;
    color: #666;
    margin-bottom: 0.5rem;
  }

  .placeholder-title {
    font-weight: 700;
    font-size: 1rem;
    margin-bottom: 0.5rem;
  }

  .placeholder-text {
    font-size: 0.9rem;
    line-height: 1.5;
    color: #555;
    margin: 0;
  }

  .result-callout {
    border-radius: 12px;
    padding: 0.9rem 1rem;
    background: #f7f7f7;
    margin: 1rem 0;
  }

  .result-callout strong {
    display: block;
    margin-bottom: 0.3rem;
  }

  .publication {
    margin: 1.15rem 0;
    padding-bottom: 1rem;
    border-bottom: 1px solid #eeeeee;
  }

  .publication:last-child {
    border-bottom: none;
  }

  .publication-title {
    font-weight: 700;
  }

  .publication-meta {
    margin-top: 0.25rem;
    color: #555;
    font-style: italic;
  }

  .btn-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 0.55rem;
  }

  .color-button {
    display: inline-block;
    padding: 0.35rem 0.7rem;
    border-radius: 999px;
    background: #eeeeee;
    color: #222;
    font-size: 0.85rem;
    line-height: 1.2;
  }

  .btn-row a {
    text-decoration: none;
  }

  .method-list {
    columns: 2;
    column-gap: 2rem;
  }

  @media (max-width: 700px) {
    .method-list {
      columns: 1;
    }
  }
</style>

<div class="research-intro">
  <p>
    I build <strong>computational methods that serve social and organizational decision-making</strong>.
    My work sits at the intersection of <strong>NLP</strong>, <strong>machine learning</strong>, and
    <strong>computational social science</strong>, with applied threads in communication, safety/health,
    and public policy. This page complements my <a href="/projects/">Projects</a> page by grouping
    publications and artifacts under the research lines they advance.
  </p>
</div>

<hr>

<h2>Themes &amp; Questions</h2>

<div class="theme-grid">
  <div class="theme-card">
    <h3>Affective meaning in digital communication</h3>
    <p>
      How do people signal and interpret emotions in text-based settings, and how can models respect
      sociocultural context?
    </p>
  </div>

  <div class="theme-card">
    <h3>Data-driven safety &amp; health</h3>
    <p>
      When do sensors, analytics, and feedback systems change behavior and reduce risk?
    </p>
  </div>

  <div class="theme-card">
    <h3>Computational policy analytics</h3>
    <p>
      What signals forecast political momentum, and how stable are relationships between money,
      polling, and campaign events?
    </p>
  </div>

  <div class="theme-card">
    <h3>Expectations in socio-economic systems</h3>
    <p>
      How do modeling choices about expectations affect stability, identifiability, and interpretation
      in macro-style systems?
    </p>
  </div>
</div>

<hr>

<h2>Publications by Research Line</h2>

<section class="research-line" id="affective-nlp">
  <div class="research-line-layout">
    <div>
      <h2> Affective Meaning &amp; NLP for Messaging</h2>

      <p>
        I combine transformer representations with affect control theory to better measure
        <strong>context-dependent emotion</strong> in chat and short text. The goal is interpretable
        affective signals that are useful for support agents, conversational systems, and social inquiry.
      </p>

      <div class="result-callout">
 This research line develops computational methods for measuring emotion and social meaning in online communication. Across three connected papers, I use Affect Control Theory (ACT) to model how emotional states shift during text-based interactions, where body language and vocal cues are absent. The work extends affective dictionaries by mapping word and emoji embeddings into ACT’s evaluation–potency–activity space, enabling models to represent not only whether language is positive or negative, but also whether it signals power, agency, intensity, or social alignment.
<br>
The main artifact from this line is a visual pipeline showing how short messages, emojis, and social-event contexts are transformed into interpretable affective representations. Early work modeled emotional transitions in chatbot-style messaging and showed how emoji representation can enrich affective lexicons for online conversations. The later BERTNN framework advances this idea by using contextual transformer embeddings to estimate affective meanings for new concepts, supporting scalable, culturally adaptive analysis of sentiment and social dynamics.
      </div>

      <div class="publication">
        <div class="publication-title">
          Contextual Embeddings in Sociological Research: Expanding the Analysis of Sentiment and Social Dynamics.
        </div>
        <div class="publication-meta">Sociological Methodology, 2024.</div>
        <div class="btn-row">
          <a href="https://journals.sagepub.com/doi/abs/10.1177/00811750241260729">
            <div class="color-button">cite</div>
          </a>
        </div>
      </div>

      <div class="publication">
        <div class="publication-title">
          Adapting Online Messaging Based on Emotional State.
        </div>
        <div class="publication-meta">UMAP ’21.</div>
        <div class="btn-row">
          <a href="https://dl.acm.org/doi/pdf/10.1145/3450613.3459661">
            <div class="color-button">pdf</div>
          </a>
          <a href="https://dl.acm.org/doi/10.1145/3450613.3459661">
            <div class="color-button">cite</div>
          </a>
        </div>
      </div>

      <div class="publication">
        <div class="publication-title">
          How emoji and word embedding helps to unveil emotional transitions during online messaging.
        </div>
        <div class="publication-meta">IEEE SysCon ’21.</div>
        <div class="btn-row">
          <a href="https://arxiv.org/ftp/arxiv/papers/2104/2104.11032.pdf">
            <div class="color-button">pdf</div>
          </a>
          <a href="https://ieeexplore.ieee.org/abstract/document/9447137">
            <div class="color-button">cite</div>
          </a>
          <a href="https://github.com/moeenm/emojis_unveil_emotions">
            <div class="color-button">code</div>
          </a>
        </div>
      </div>
    </div>

    <aside class="research-visual">
        <img src="/images/affectiveNLP.jpg" alt="Effect of interactions on affective meanings">
        <p class="placeholder-text">Affect Control Theory (ACT) estimates affective meanings from contextual interactions.
      </p>
    </aside>
  </div>
</section>

<section class="research-line" id="safety-health">
  <div class="research-line-layout">
    <div>
      <h2> Safety, Sensors &amp; Behavior Change</h2>

      <p>
        From <strong>RFID+haptics</strong> for collision warnings to <strong>telematics-guided eco-driving</strong>
        and <strong>sleep technology</strong> feasibility, I study how analytics and design can
        <strong>reduce risk</strong> and support healthier behavior in the wild.
      </p>

      <div class="result-callout">
         
        The RFID collision-warning study reported collision prediction with <strong>less than 14% false alarms</strong>.
        In the Mindful Driving project, linked UVA coverage reported nearly <strong>6% fuel-economy improvement</strong>,
        more than <strong>23 gallons of fuel saved per vehicle</strong>, and <strong>457 pounds of annual greenhouse-gas
        reductions per vehicle</strong>.
      </div>

      <div class="publication">
        <div class="publication-title">
          Collision Prediction and Prevention in Contact Sports Using RFID Tags and Haptic Feedback.
        </div>
        <div class="publication-meta">AHFE Wearable &amp; Assistive Technology, 2021.</div>
        <div class="btn-row">
          <a href="https://link.springer.com/chapter/10.1007/978-3-030-80091-8_47">
            <div class="color-button">cite</div>
          </a>
        </div>
      </div>

      <div class="publication">
        <div class="publication-title">
          Safe and Sustainable Fleet Management with Data Analytics and Training.
        </div>
        <div class="publication-meta">Systems and Information Engineering Design Symposium (SIEDS), 2021.</div>
        <div class="btn-row">
          <a href="https://www.fm.virginia.edu/about/news/mindful-driving.html">
            <div class="color-button">coverage</div>
          </a>
        </div>
      </div>

      <div class="publication">
        <div class="publication-title">
          Preliminary feasibility of technology use in an internet-delivered intervention:
          Improving sleep in older adults with mild cognitive impairment.
        </div>
        <div class="publication-meta">Alzheimer’s &amp; Dementia, conference abstract, 2020.</div>
        <div class="btn-row">
          <a href="https://alz-journals.onlinelibrary.wiley.com/doi/epdf/10.1002/alz.038831">
            <div class="color-button">pdf</div>
          </a>
          <a href="https://alz-journals.onlinelibrary.wiley.com/doi/abs/10.1002/alz.038831">
            <div class="color-button">cite</div>
          </a>
        </div>
      </div>
    </div>

    <aside class="research-visual">
        <img src="/images/collision.jpg" alt="Sensor and telematics analytics for safety and behavior change">
        <p class="placeholder-text">Tracking playes on the field.
      </p>
    </aside>
  </div>
</section>

<section class="research-line" id="policy-analytics">
  <div class="research-line-layout">
    <div>
      <h2> Computational Policy Analytics</h2>

      <p>
        Using time-segmented models such as <strong>joinpoint regression</strong>, I examine how
        <strong>fundraising and polling</strong> co-evolve in U.S. primary campaigns and what those dynamics
        imply for forecasting, momentum, and resource allocation.
      </p>

      <div class="result-callout">
         
        This work compares polling and financial contributions during the 2020 Democratic primaries and uses
        change-point analysis to identify moments when campaign trajectories shift, including shifts associated
        with debate performance and candidate support.
      </div>

      <div class="publication">
        <div class="publication-title">
          A Tale of Two Metrics: Polling and Financial Contributions as a Measure of Performance.
        </div>
        <div class="publication-meta">IEEE SysCon ’21.</div>
        <div class="btn-row">
          <a href="https://ieeexplore.ieee.org/abstract/document/9483746">
            <div class="color-button">cite</div>
          </a>
          <a href="https://arxiv.org/abs/2103.12984">
            <div class="color-button">preprint</div>
          </a>
        </div>
      </div>
    </div>

    <aside class="research-visual">
        <img src="/images/two_metrics_joinpoint.png" alt="M">
      <p class="placeholder-text">
        Polling + fundraising change points.
      </p>
    </aside>
  </div>
</section>

<section class="research-line" id="expectations-systems">
  <div class="research-line-layout">
    <div>
      <h2> Expectations &amp; Macro-Style Systems</h2>

      <p>
        My early work studied <strong>expectation formation</strong> and solution properties in macro-style systems,
        with emphasis on stability, interpretability, and plausible micro-foundations.
      </p>

      <div class="result-callout">
         
         <p>
  This research line studies how assumptions about <strong>expectation formation</strong>
  affect the stability and interpretation of macro-style dynamic systems. In the rational
  expectations literature, the determinacy condition is often used as a criterion for
  identifying unique stable solutions. My early work revisits this assumption and argues
  that determinacy alone can be a weak or insufficient criterion, especially when the
  mathematical structure of the model does not fully capture how agents form and revise
  expectations.
</p>

<p>
  The related multi-agent work proposes an alternative way to model systems with linear
  rational expectations by representing decision makers as predictive agents rather than
  relying only on centralized equilibrium conditions. In this view, agents estimate future
  states, optimize their own actions, and interact through system-level feedback. A useful
  visual artifact for this line would show the contrast between a traditional rational
  expectations equation and the behind-the-scenes agent-based process that generates
  expectations, decisions, and stable system behavior.
</p>
      </div>

      <div class="publication">
        <div class="publication-title">
          Why the determinacy condition is a weak criterion in rational expectations models.
        </div>
        <div class="publication-meta">International Conference on Business and Economics Research, 2010.</div>
      </div>

      <div class="publication">
        <div class="publication-title">
          A predictive multi-agent approach to model systems with linear rational expectations.
        </div>
        <div class="publication-meta">First Iranian Economic Conference, 2011.</div>
      </div>
    </div>

    <aside class="research-visual">
        <img src="/images/RE.png" alt="Multi-agent expectation formation and macro-system feedback loops">
        <p class="placeholder-text">Behind the Rational Expectation equations.
      </p>
    </aside>
  </div>
</section>

<hr>

<h2>Methods &amp; Tooling</h2>

<ul class="method-list">
  <li><strong>NLP:</strong> contextual embeddings, BERT-family models, lexicon expansion, sequence modeling for affect.</li>
  <li><strong>ML:</strong> regression/classification, clustering, time-series segmentation, subgroup-aware evaluation.</li>
  <li><strong>Sensing &amp; Systems:</strong> telematics analytics, RFID localization, dashboarding, training feedback.</li>
  <li><strong>Policy analytics:</strong> campaign-performance signals, joinpoint regression, comparative trend analysis.</li>
  <li><strong>Open materials:</strong> selected code and preprints linked above; additional items available on request.</li>
</ul>

<hr>

<h2>Impact &amp; Collaboration</h2>

<ul>
  <li>
    <strong>Mindful Driving:</strong> supported by a Jefferson Trust grant; cross-unit work with operations and fleet
    partners; linked coverage reports improved fuel economy and greenhouse-gas reductions from the deployed software
    comparison.
  </li>
  <li>
    <strong>Affective NLP:</strong> published in a sociological methods venue, reflecting interdisciplinary work across
    NLP, social psychology, and computational social science.
  </li>
  <li>
    Collaborations across <strong>sociology, economics, kinesiology, nursing, political science, data science, business,
    and engineering</strong>.
  </li>
</ul>

<hr>

<h2>Pointers</h2>

<div class="btn-row">
  <a href="https://scholar.google.com/citations?user=BtO9RngAAAAJ&hl=en">
    <div class="color-button">Google Scholar</div>
  </a>
  <a href="/projects/">
    <div class="color-button">Projects</div>
  </a>
  <a href="/about/">
    <div class="color-button">About</div>
  </a>
</div>
