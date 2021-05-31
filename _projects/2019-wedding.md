---
title: Travel-themed wedding
gist: That was amazing! We had an amazing wedding! We flew on a plane.
image: /images/pic01.jpg
rows:
  - columns:
    - image: /images/pic01.jpg
      size: 6
    - size: 6
      text: >-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque euismod libero ac arcu semper, id feugiat sapien tempus. 
        Etiam venenatis bibendum tortor, in tempor purus tincidunt vel. Morbi tristique lectus vel ante sollicitudin ultricies et nec ligula. 
        Quisque eu nulla eget tortor interdum porta id sed ante. Curabitur a nunc dolor. In sodales enim ac ex scelerisque, sit amet pretium est mollis. 
        Curabitur quis magna id velit ullamcorper volutpat. Mauris id nisl ut ligula ultricies molestie. Nulla eget consequat tellus. In hac habitasse platea dictumst.
  - columns:
    - size: 8
      text: >-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque euismod libero ac arcu semper, id feugiat sapien tempus. 
        Etiam venenatis bibendum tortor, in tempor purus tincidunt vel. Morbi tristique lectus vel ante sollicitudin ultricies et nec ligula. 
        Quisque eu nulla eget tortor interdum porta id sed ante. Curabitur a nunc dolor. In sodales enim ac ex scelerisque, sit amet pretium est mollis. 
        Curabitur quis magna id velit ullamcorper volutpat. Mauris id nisl ut ligula ultricies molestie. Nulla eget consequat tellus. In hac habitasse platea dictumst.
    - image: /images/pic02.jpg
      size: 4
  - columns:
    - size: 3
      image: /images/pic03.jpg
    - size: 6
      text: >-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque euismod libero ac arcu semper, id feugiat sapien tempus. 
        Etiam venenatis bibendum tortor, in tempor purus tincidunt vel. Morbi tristique lectus vel ante sollicitudin ultricies et nec ligula. 
        Quisque eu nulla eget tortor interdum porta id sed ante. Curabitur a nunc dolor. In sodales enim ac ex scelerisque, sit amet pretium est mollis. 
        Curabitur quis magna id velit ullamcorper volutpat. Mauris id nisl ut ligula ultricies molestie. Nulla eget consequat tellus. In hac habitasse platea dictumst.
    - image: /images/pic01.jpg
      size: 3
  - columns:
    - image: /images/pic01.jpg
      size: 6
    - image: /images/pic02_vert.jpg
      size: 3
    - image: /images/pic01_vert.jpg
      size: 3

---


{% for row in page.rows %}
<section>
    <div class="container">
        <div class="row">
            {% for col in row.columns %}
            <div class="col-{{ col.size }}">
            {% if col.image" %}
                <span class="image fit"><img src=" {{ col.image }}"/></span>
            {% endif %}
            {% if col.text" %}
                <p>{{ col.text }}</p>
            {% endif %}
            </div>
            {% endfor %}
        </div>
    </div>
</section>
{% endfor %}
