---
---
Analytic Imaging Diagnostics Arena ([AIDA](https://medtech4health.se/aida)) is a
Swedish arena for research and innovation on artificial intelligence, AI, for
medical image analysis. Here, academia, healthcare and industry meet to
translate technical advances in AI technology into patient benefit in the form
of clinically useful tools.

The most important factor for training world-class AI is access to massive
amounts of high-quality training data.
The [AIDA data hub](https://medtech4health.se/aida/datahub/) is a place where
researchers can collaboratively gather, annotate, share and enrich large volumes
of research data for machine learning in medical imaging diagnostics. This site
provides information on the datasets that have been shared on the AIDA data hub,
and make them findable and citeable using Digital Object identifiers
([DOI](https://www.doi.org/)).

{% assign total = 0 %}
{% for d in site.datasets %}{% assign total = total | plus: d.other.bytes %}{% endfor %}
Thus far <b>{% include human_friendly_filesize bytes=total %} </b> image data from radiology
and pathology has been shared on the AIDA data hub.

*The AIDA data hub is currently being developed in collaboration with pilot
users from research, clinic and industry. It is planned to go into production
phase within June 2019.* 

## Datasets shared on the AIDA data hub

<div class="dataset-table">
  <table>
    <tr>
      <th>DOI</th>
      <th>Title</th>
      <th>Year</th>
    </tr>
    {% for d in site.datasets %}
      <tr>
        <td>{{ d.title }}</td>
        <td><a href="{{ d.url }}">{{ d.datacite.name }}</a></td>
        <td>{{ d.datacite.publicationYear }}</td>
      </tr>
    {% endfor %}
  </table>
</div>

The information on these datasets is also available in machine-readable form
through an [api](api/).
