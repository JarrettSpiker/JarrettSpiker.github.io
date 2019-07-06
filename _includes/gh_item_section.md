<details open><summary>Expand...</summary>
{%- for item1 in site.data.gloomhaven.items -%}
    {%- assign itemLevel = item1.level | downcase %}
    {%- if itemLevel == include.level -%}
        {% include gh_item.html itemObj=item1 cardRange=include.cardRange%}
    {%- endif -%}
{%- endfor -%}
</details>
<br/>
<br/>