---
layout: default
---

### Training

{% assign data=site.data.osgeouk_training %}

<table>
    <thead>
    {% for column in data[0] %}
        <th>{{ column[0] | capitalize }}</th>
    {% endfor %}
    </thead>
    <tbody>
    {% for row in data %}
        <tr>
        {% for cell in row %}
            <td>
            {% if cell[1] contains 'http' %}
                <a href="{{ cell[1] }}">More info</a>
            {% else %}
                {{ cell[1] }}
            {% endif %}
            </td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>

#### Adding courses

To add courses to this page: sign-up for a GitHub account, edit [osgeouk_training.csv](https://github.com/osgeouk/website/blob/gh-pages/_data/osgeouk_training.csv) to include your courses and submit a pull request.
