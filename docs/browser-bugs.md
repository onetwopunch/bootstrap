---
layout: default
title: Wall of browser bugs
---

Bootstrap currently works around several outstanding browser bugs in major browsers to deliver the best cross-browser experience possible. Some bugs, like those listed below, cannot be solved by us.

We publicly list browser bugs that are impacting us here, in the hopes of expediting the process of fixing them. For information on Bootstrap's browser compatibility, [see our browser compatibility docs](../getting-started/#support).

<div class="table-responsive">
  <table class="bs-docs-browser-bugs table table-bordered table-hover">
    <thead>
      <tr>
        <th>Browser(s)</th>
        <th>Summary of bug</th>
        <th>Upstream bug(s)</th>
        <th>Bootstrap issue(s)</th>
      </tr>
    </thead>
    <tbody>
      {% for bug in site.data.browser-bugs %}
      <tr>
        <td>{{ bug.browser }}</td>
        <td>{{ bug.summary | markdownify | bugify }}</td>
        <td>{{ bug.upstream_bug | bugify }}</td>
        <td>{{ bug.origin | bugify }}</td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>