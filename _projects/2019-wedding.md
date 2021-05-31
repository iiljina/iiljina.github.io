---
title: Travel-themed wedding
gist: That was amazing! We had an amazing wedding! We flew on a plane.
image: /images/pic01.jpg
all_images:
    - image_size: 6
      images:
        - url: /images/pic01.jpg
          text: "my image 01"
        - url: /images/pic03.jpg
          text: "my image 03"
    - image_size: 4
      images:
        - url: /images/pic01.jpg
          text: "my image 01"  
        - url: /images/pic02.jpg
          text: "my image 02"
        - url: /images/pic03.jpg
          text: "my image 03"
---

<span class="image left">![pic03_bigger]</span>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque euismod libero ac arcu semper, id feugiat sapien tempus. 
Etiam venenatis bibendum tortor, in tempor purus tincidunt vel. Morbi tristique lectus vel ante sollicitudin ultricies et nec ligula. 
Quisque eu nulla eget tortor interdum porta id sed ante. Curabitur a nunc dolor. In sodales enim ac ex scelerisque, sit amet pretium est mollis. 
Curabitur quis magna id velit ullamcorper volutpat. Mauris id nisl ut ligula ultricies molestie. Nulla eget consequat tellus. In hac habitasse platea dictumst.

<span class="image right">![pic03_smaller]</span>
Morbi tempor egestas purus quis fermentum. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. 
In eu elit mattis, facilisis augue non, eleifend ante. Etiam gravida varius risus. In tincidunt est at efficitur eleifend. 
Curabitur a ligula vehicula, efficitur ligula molestie, pulvinar enim. Aliquam erat volutpat. Suspendisse dignissim, elit id faucibus molestie, urna justo tempor libero, ut rhoncus lorem odio at velit. 
Mauris aliquet velit quis diam tristique, ut vulputate mauris semper. Aliquam viverra malesuada elit, eget interdum purus faucibus non.

<span class="image fit">![pic03]</span>
Integer volutpat orci vel leo rutrum, eu tempor diam dictum. Aliquam velit libero, consequat non nunc non, vestibulum tincidunt massa. 
Proin iaculis sagittis nunc. Sed hendrerit urna nibh, quis euismod tellus pretium et. Pellentesque et sagittis enim, vel luctus neque. 
Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vestibulum a ultrices enim, vel malesuada tellus. 
Praesent ut dapibus dui. Nam at viverra purus. Curabitur aliquet nisi eget suscipit fermentum. Integer sollicitudin ante ac odio suscipit eleifend eget et nibh.

<span class="image left">![pic03_bigger]</span>
Nam et placerat tellus. Aenean at iaculis elit. Cras tincidunt turpis dui, viverra feugiat sapien gravida sed. 
Pellentesque dolor sem, feugiat sed nulla sed, elementum varius sapien. Pellentesque ut pharetra urna. Donec laoreet maximus pellentesque. 
Phasellus at tincidunt massa. Sed in egestas augue. Fusce sed tristique mauris, a lobortis augue. Sed faucibus dapibus lacus at condimentum. Duis id sapien at nulla suscipit facilisis non in mi.

<span class="image right">![pic03]</span>
Maecenas non neque ligula. Morbi suscipit nibh id magna varius pellentesque. Donec eu ante vitae lacus maximus eleifend vel at neque. 
Nunc aliquet suscipit nunc, vitae finibus elit tincidunt non. Integer pellentesque nisi consectetur risus dignissim, sit amet tincidunt nibh elementum. 
Cras nec vehicula sem, non aliquet mauris. Vestibulum dui mauris, elementum et luctus ut, finibus vel magna. Fusce id sapien blandit, ullamcorper nisl a, fermentum libero. 
Aliquam eros sem, sagittis ut tortor sed, laoreet dapibus diam. In ac turpis urna.


See all pictures
===

<div class="box alt">
{% for row in page.all_images %}
<div class="row">
    {% for col in row.images %}
    <div class="col-{{ row.image_size }}"><span class="image fit"><img src="{{ col.url }}" alt="{{ col.text }}"/></span></div>
    {% endfor %}
</div>
{% endfor %}
</div>

[pic03]: /images/pic03.jpg
{: height="250px" width="250px"}

[pic03_smaller]: /images/pic03.jpg
{: height="150px" width="150px"}

[pic03_bigger]: /images/pic03.jpg
{: height="550px" width="550px"}

