---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

This page is collecting open source activities of [Melown Technologies
SE](http://melown.com) as well as gives brief overview about the content of [Melown's
GitHub](https://github.com/melown), so you can start using the 3D libraries for
both - the server and the client - and help to maintain our generic
documentation and format specs. For complete list of
tools, look  at [Projects](/projects) page.

If not stated otherwise, all tools are published under the [BSD 2-Clause
license](https://opensource.org/licenses/BSD-2-Clause). *NOTE: Always check the
LICENSE file in each project.*

<div class="container">

<div class="row">

{% for my_page in site.pages %}
  {% if my_page.layout == 'component' %}
  <div class="col-md-4">
  <div class="panel panel-default">
  
  <div class="panel-heading"><a href="{{ my_page.url | relative_url }}">{{ my_page.title | escape }}</a></div>
  <div class="panel-body">

          {{ my_page.description }}

          <p>
          <a class="btn btn-default" href="{{ my_page.url | relative_url }}" role="button">View details &raquo;</a>
          </p>
  </div> <!-- panel-body -->
  </div> <!-- panel -->
  </div> <!-- col-md4 -->
  {% endif %}
{% endfor %}


</div><!-- row -->
</div> <!-- container -->
