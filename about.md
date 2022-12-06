---
layout: page
title: About
permalink: /about/
---

This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)

# Lorem Ipsum - Dolor
													
## Sit Amet  
**1. Consectetur (tempor):** 2022-05-16   
**2. Adipiscing (sed do eiusmod):** v1.0  
**3. Incididunt:** Jane Doe, John Doe, Johann Doe  
**4. Ut labore et dolore magna aliqua?   
    a.	Odio <sup>1</sup>:** Quis commodo odio aenean seds  
    **b. Morbi  (optional):** Posuere urna nec tincidunt praesent semper feugiat.  
**5. Tempor nec feugiat nisl pretium fusce?**  
    **a.	Odio<sup>1</sup>:** Et magnis dis parturient montes nascetur ridiculus mus mauris vitae.  
    **b.	Nulls (facilisi):** Nulla facilisi morbi tempus iaculis urna id.  
 **6. Nam at lectus urna duis convallis convallis tellus id?**  
    **a.	Odio<sup>1</sup>:** Urna; duis  
    **b.	Pulvinar (neque):** Ut faucibus pulvinar elementum integer enim neque volutpat   
 **7. Ut pharetra:** 99 Amet  
<sup>*1</sup> Vel pretium lectus quam id leo in vitae.*

## Sit Amet 
**Consectetur Adipiscing [ABCs](https://www.google.com/):**  
DEF: 12345678 (Elit Duis / Tristique, sollicitudin nib)

**Habitant:**  
GHI1234567 (morbi tristique)  
GHI8912345 (morbi tristique V2)  
GHI6789123 (morbi tristique)
	
### **Senectus Et**

99B Nibh venenatis cras sed felis eget velit aliquet sagittis id. A arcu cursus vitae congue mauris rhoncus. Venenatis tellus in metus vulputate eu. Elit eget gravida cum sociis natoque penatibus et. At in tellus integer feugiat. Lacus vestibulum sed arcu non odio euismod lacinia at. Felis donec et odio pellentesque diam. Nulla facilisi cras fermentum odio eu feugiat. Suspendisse in est ante in nibh mauris cursus mattis molestie. Nisl suscipit adipiscing bibendum est ultricies integer.

### **Bibendum Est**

**Ultricies Integer**  
Vitae congue mauris rhoncus aenean vel elit scelerisque mauris pellentesque. Pharetra pharetra massa massa ultricies. Cras semper auctor neque vitae tempus. Scelerisque eleifend donec pretium vulputate sapien nec sagittis aliquam. Sit amet facilisis magna etiam tempor orci. A condimentum vitae sapien pellentesque habitant morbi tristique.

**Mi Ipsum**  
Faucibus vitae aliquet nec ullamcorper sit amet. Pellentesque adipiscing commodo elit at. Cum sociis natoque penatibus et magnis dis parturient montes nascetur. Orci nulla pellentesque dignissim enim sit amet venenatis urna. Ipsum a arcu cursus vitae congue mauris rhoncus.

**Aliquet**  
Justo nec ultrices dui sapien eget mi. Aliquam malesuada bibendum arcu vitae. Consequat ac felis donec et odio pellentesque diam volutpat. Ut tellus elementum sagittis vitae et.

## **Antibodies**  
* ~~*N/A*~~

![Placeholder image](/assets/placeholder.png)

{% include about.md items="lorem, ipsum" file="data/directory-schema_spatialseq_v1.yaml" caption="Directory Structure" %}
{% assign tableItems = include.items | split: ", " %}
{% assign tableFileParam = {{include.file}} %}
{% assign tableFile = site.data[tableFileParam] %}

<table class="grid" style="width: 100%">
    <caption>{{include.caption}}</caption>
    <colgroup>
        <col width="16%" />
        <col width="16%" />
        <col width="16%" />
        <col width="16%" />
        <col width="16%" />
        <col width="20%" />
    </colgroup>
    <thead>
        <tr class="header">
            <th>File</th>
            <th>File type</th>
            <th>Directory</th>
            <th>Input file or precursor data</th>
            <th>Generator program or pipeline with URL</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
    {% for entry in tableItems %}
        <tr>
          <td>{{ tableFile[entry].field }}<br/>
          {% if tableFile[entry].required == true %}<span class="tableRequired">required</span>{% endif %}</td>
          <td>{{tableFile[entry]description}}
          {% if tableFile[entry].values != empty %}{{ tableFile[entry].values }}{% endif %}</td>
          <td>{{ tableFile[entry].type }}</td>
        </tr>
    {% endfor %}
    </tbody>
</table>
															
# Elementum-nibh

## Tellus molestie Nunc

### **Non blandit**

---
Sem et :
  - Consequat Id:malesuada
    Pellentesque:0
    Gravida?:yes
    Viverra:Praesent tristique magna sit amet purus gravida quis
  - Consequat Id:img
    Pellentesque:0
    Viverra?:yes
    Description:Nisi lacus sed viverra tellus in hac habitasse.
  - Consequat Id:lab
    Pellentesque:1
    Viverra?:yes
    Gravida:Nisi lacus sed viverra tellus in hac habitasse.
  - Consequat Id:lab/processed
    Pellentesque:1.1
    Gravida?:yes
    Gravida:Diam volutpat commodo sed egestas egestas fringilla phasellus faucibus scelerisque.
  - Consequat Id:hive
    Pellentesque:2
    Gravida?:yes
    Gravida:Duis at tellus at urna condimentum mattis pellentesque id nibh.
---
