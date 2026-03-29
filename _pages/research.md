---
layout: default
title: "Research Areas"
permalink: /research/
---

<!-- TODO: add sections on TPG, env opt, and learning-based MAPF -->

<div class="page-wrapper">
  <h1>Research Areas</h1>

  <div class="research-intro">
    <p>
      Our research focuses on developing fundamental algorithms that enable large teams of autonomous agents
      to accomplish collaborative tasks intelligently in dynamic environments.
    </p>
  </div>
  <div class = "info-wrapper">
    A summary of our ongoing research can be found
    <a href="/files/jiaoyangli/ARCS-2024-Orientation-Poster.pdf">here</a>.
    <span class="info-wrapper-note">Updated: August 2024</span>
  </div>

  <nav class="page-nav">
    <a href="#mapf">MAPF</a>
    <a href="#warehouse">Warehouses</a>
    <a href="#arm">Multi-Arm</a>
    <a href="#envopt">Environment Optimization</a>
    <a href="#execution">Execution</a>
    <a href="#traffic">Traffic Management</a>
  </nav>

  <section class="research-area" id="mapf">
    <div class="research-area-media">
      <img src="/files/jiaoyangli/images/mapf-demo.gif" alt="MAPF demo" />
    </div>
    <div class="research-area-content">
      <h3>Multi-Agent Path Finding (MAPF)</h3>
      <p>
        We aim to develop principled algorithms to solve challenging MAPF instances
        via a variety of AI and optimization technologies, such as
        constraint reasoning, heuristic search, stochastic local search, and machine learning.
      </p>
      <ul class="research-links">
        <li><a href="/mapf">Research overview on MAPF algorithms</a> <span>[updated: September 2022]</span></li>
        <li><a href="/mamp">Research overview on generalizing MAPF for various multi-robot systems</a> <span>[updated: May 2025]</span></li>
      </ul>
      <details class="research-publications">
        <summary>Relevant publications</summary>
        <ul>
          {% for pub in site.data.pubs %}
            {% if pub.tags contains "mapf" %}
              {% include pub-list.html %}
            {% endif %}
          {% endfor %}
        </ul>
      </details>
    </div>
  </section>

  <section class="research-area" id="warehouse">
    <div class="research-area-media">
      <img src="/files/jiaoyangli/images/warehouse-5x.gif" alt="Automated warehouse robots" />
    </div>
    <div class="research-area-content">
      <h3>Coordination of Large Robot Teams in Automated Warehouses</h3>
      <p>
        We aim to combine task planning, path planning, and execution
        to coordinate thousands of mobile robots to fulfill delivery tasks in automated warehouses.
      </p>
      <ul class="research-links">
        <li><a href="/warehouse">Research overview</a> <span>[updated: September 2022]</span></li>
      </ul>
      <details class="research-publications">
        <summary>Relevant publications</summary>
        <ul>
          {% for pub in site.data.pubs %}
            {% if pub.tags contains "warehouse" %}
              {% include pub-list.html %}
            {% endif %}
          {% endfor %}
        </ul>
      </details>
    </div>
  </section>

  <section class="research-area" id="arm">
    <div class="research-area-media">
      <img src="/files/jiaoyangli/images/bar.gif" alt="Multi-robotic-arm manipulation" />
    </div>
    <div class="research-area-content">
      <h3>Multi-Robotic-Arm Cooperative Manipulation</h3>
      <p>
        We aim to develop combined task planning, motion planning, and execution frameworks
        to jointly plan safe, low-cost plans
        for a team of robotic arms to perform cooperative manipulation and assembly.
      </p>
      <ul class="research-links">
        <li><a href="https://intelligent-control-lab.github.io/APEX-MR/">Dual-arm lego assembly</a> <span>[updated: January 2025]</span></li>
        <li><a href="/arm">Research overview</a> <span>[updated: September 2022]</span></li>
      </ul>
      <details class="research-publications">
        <summary>Relevant publications</summary>
        <ul>
          {% for pub in site.data.pubs %}
            {% if pub.tags contains "arm" %}
              {% include pub-list.html %}
            {% endif %}
          {% endfor %}
        </ul>
      </details>
    </div>
  </section>

  <section class="research-area" id="envopt">
    <div class="research-area-media">
      <img src="/files/jiaoyangli/images/envopt-overview.gif" alt="Environment optimization overview" />
    </div>
    <div class="research-area-content">
      <h3>Environment Optimization for Fostering Agent Collaboration</h3>
      <p>
        While traditional research in multi-agent systems focuses on improving agents' algorithms under fixed environmental settings,
        our team takes a complementary perspective: We aim to optimize the environment itself to enhance multi-agent performance.
      </p>
      <ul class="research-links">
        <li><a href="/envopt">Research overview</a> <span>[updated: May 2025]</span></li>
      </ul>
      <details class="research-publications">
        <summary>Relevant publications</summary>
        <ul>
          {% for pub in site.data.pubs %}
            {% if pub.tags contains "envopt-physical" or  pub.tags contains "envopt-virtual" %}
              {% include pub-list.html %}
            {% endif %}
          {% endfor %}
        </ul>
      </details>
    </div>
  </section>

  <section class="research-area" id="execution">
    <div class="research-area-media">
      <img src="/files/jiaoyangli/images/sync-vs-async.gif" alt="Execution overview" />
    </div>
    <div class="research-area-content">
      <h3>From Plan to Reality: Robust Execution for Multi-Robot Systems</h3>
      <p>
        While state-of-the-art MAPF planners can generate collision-free paths for hundreds or even thousands of agents within seconds,
        they often overlook critical real-world factors, such as robot dynamics, timing constraints, and execution uncertainty.
        We aim to bridge this gap by developing a robust and safe multi-robot planning and execution framework
        that can reliably execute MAPF-generated plans, even when those plans are imperfect or subject to real-world disturbances.
      </p>
      <ul class="research-links">
        <li><a href="/execution">Research overview</a> <span>[updated: May 2025]</span></li>
      </ul>
      <details class="research-publications">
        <summary>Relevant publications</summary>
        <ul>
          {% for pub in site.data.pubs %}
            {% if pub.tags contains "execution" %}
              {% include pub-list.html %}
            {% endif %}
          {% endfor %}
        </ul>
      </details>
    </div>
  </section>

  <section class="research-area" id="traffic">
    <div class="research-area-media">
      <img src="/files/jiaoyangli/images/flatland.gif" alt="Traffic management" />
    </div>
    <div class="research-area-content">
      <h3>Intelligent Traffic Management</h3>
      <p>
        We aim to develop intelligent planning systems to coordinate
        trains, airplanes, autonomous vehicle, etc. on complex road networks under uncertainty.
      </p>
      <ul class="research-links">
        <li><a href="/traffic">Research overview</a> <span>[updated: September 2022]</span></li>
      </ul>
      <details class="research-publications">
        <summary>Relevant publications</summary>
        <ul>
          {% for pub in site.data.pubs %}
            {% if pub.tags contains "traffic" %}
              {% include pub-list.html %}
            {% endif %}
          {% endfor %}
        </ul>
      </details>
    </div>
  </section>
</div>