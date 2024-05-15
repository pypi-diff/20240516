# Comparing `tmp/django_sh-1.0.8-py3-none-any.whl.zip` & `tmp/django_sh-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1485589 bytes, number of entries: 621
+Zip file size: 1485606 bytes, number of entries: 621
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-15 17:30 django_sh/__init__.py
 -rw-r--r--  2.0 unx      395 b- defN 21-Sep-15 16:45 django_sh/asgi.py
 -rw-r--r--  2.0 unx     3281 b- defN 21-Sep-15 17:41 django_sh/settings.py
 -rw-r--r--  2.0 unx      797 b- defN 21-Sep-15 17:39 django_sh/urls.py
 -rw-r--r--  2.0 unx      395 b- defN 21-Sep-15 16:45 django_sh/wsgi.py
--rw-r--r--  2.0 unx       58 b- defN 21-Sep-21 22:10 sh/__init__.py
+-rw-r--r--  2.0 unx       58 b- defN 21-Sep-21 22:12 sh/__init__.py
 -rw-r--r--  2.0 unx       63 b- defN 21-Sep-14 02:19 sh/admin.py
 -rw-r--r--  2.0 unx       79 b- defN 21-Sep-14 02:19 sh/apps.py
 -rw-r--r--  2.0 unx     1189 b- defN 21-Sep-21 22:02 sh/models.py
 -rw-r--r--  2.0 unx       60 b- defN 21-Sep-14 02:19 sh/tests.py
 -rw-r--r--  2.0 unx      715 b- defN 21-Sep-15 23:16 sh/urls.py
 -rw-r--r--  2.0 unx     3583 b- defN 21-Sep-21 22:10 sh/views.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-15 17:43 sh/management/__init__.py
@@ -608,16 +608,16 @@
 -rw-r--r--  2.0 unx     2142 b- defN 21-Sep-14 02:19 sh/static/sh/codemirror/theme/vibrant-ink.css
 -rw-r--r--  2.0 unx     3033 b- defN 21-Sep-14 02:19 sh/static/sh/codemirror/theme/xq-dark.css
 -rw-r--r--  2.0 unx     2255 b- defN 21-Sep-14 02:19 sh/static/sh/codemirror/theme/xq-light.css
 -rw-r--r--  2.0 unx     1884 b- defN 21-Sep-14 02:19 sh/static/sh/codemirror/theme/yeti.css
 -rw-r--r--  2.0 unx     3075 b- defN 21-Sep-14 02:19 sh/static/sh/codemirror/theme/yonce.css
 -rw-r--r--  2.0 unx     2001 b- defN 21-Sep-14 02:19 sh/static/sh/codemirror/theme/zenburn.css
 -rwxr-xr-x  2.0 unx     2630 b- defN 21-Sep-21 22:06 sh/templates/sh/command.html
--rw-r--r--  2.0 unx     1367 b- defN 21-Sep-21 22:03 sh/templates/sh/command_history.html
+-rw-r--r--  2.0 unx     1405 b- defN 21-Sep-21 22:12 sh/templates/sh/command_history.html
 -rwxr-xr-x  2.0 unx     3039 b- defN 21-Sep-15 17:54 sh/templates/sh/layout.html
 -rw-r--r--  2.0 unx     1154 b- defN 21-Sep-15 23:37 sh/templates/sh/saved_commands.html
 -rwxr-xr-x  2.0 unx     2339 b- defN 21-Sep-21 16:25 sh/templates/sh/settings.html
--rw-r--r--  2.0 unx      645 b- defN 21-Sep-21 22:10 django_sh-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-21 22:10 django_sh-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Sep-21 22:10 django_sh-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    62666 b- defN 21-Sep-21 22:10 django_sh-1.0.8.dist-info/RECORD
-621 files, 4650079 bytes uncompressed, 1383757 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx      645 b- defN 21-Sep-21 22:12 django_sh-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Sep-21 22:12 django_sh-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 21-Sep-21 22:12 django_sh-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    62666 b- defN 21-Sep-21 22:12 django_sh-1.0.9.dist-info/RECORD
+621 files, 4650117 bytes uncompressed, 1383774 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -1845,20 +1845,20 @@
 
 Filename: sh/templates/sh/saved_commands.html
 Comment: 
 
 Filename: sh/templates/sh/settings.html
 Comment: 
 
-Filename: django_sh-1.0.8.dist-info/METADATA
+Filename: django_sh-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: django_sh-1.0.8.dist-info/WHEEL
+Filename: django_sh-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: django_sh-1.0.8.dist-info/top_level.txt
+Filename: django_sh-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: django_sh-1.0.8.dist-info/RECORD
+Filename: django_sh-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sh/__init__.py

```diff
@@ -1,3 +1,3 @@
 """Django shell app for browser"""
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
```

## sh/templates/sh/command_history.html

```diff
@@ -15,16 +15,16 @@
                         <th></th>
                     </tr>
                 </thead>
                 <tbody>
                     
                     {% for obj in objects %}
                     <tr>
-                        <td><a href="{% url 'sh:command' obj.pk %}">{{ obj.start }}</a></td>
-                        <td><a href="{% url 'sh:command' obj.pk %}">{{ obj.end }}</a></td>
+                        <td><a href="{% url 'sh:command' obj.pk %}">{{ obj.start|date:"d/m/Y H:i:s" }}</a></td>
+                        <td><a href="{% url 'sh:command' obj.pk %}">{{ obj.end|date:"d/m/Y H:i:s" }}</a></td>
                         <td><a href="{% url 'sh:command' obj.pk %}">{{ obj.text|truncatechars:100 }}</a></td>
                         <td><a href="{% url 'sh:command' obj.pk %}">{{ obj.user|default:"" }}</a></td>
                         <td class="text-right">
                             <a href="{% url 'sh:save_command' obj.pk %}" class="btn btn-sm">Guardar en favoritos</a>
                         </td>
                     </tr>
                     {% endfor %}
```

### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends 'sh/layout.html' %} {% load static %} {% block contenido %}
-IInniicciioo       FFiinn           CCoommaannddoo                 UUssuuaarriioo
-                           _{                       _{
-_{_{_ _o_b_j_._s_t_a_r_t _{_{_ _o_b_j_._e_n_d_ _}_} _{                       _{                 _G_u_a_r_d_a_r_ _e_n
-_}_}                         _o_b_j_._t_e_x_t_|_t_r_u_n_c_a_t_e_c_h_a_r_s_: _o_b_j_._u_s_e_r_|_d_e_f_a_u_l_t_: _f_a_v_o_r_i_t_o_s
-                           _1_0_0_ _}_}                  _"_"_ _}_}
+IInniicciioo          FFiinn           CCoommaannddoo                 UUssuuaarriioo
+_{               _{             _{                       _{
+_{               _{             _{                       _{                 _G_u_a_r_d_a_r
+_o_b_j_._s_t_a_r_t_|_d_a_t_e_: _o_b_j_._e_n_d_|_d_a_t_e_: _o_b_j_._t_e_x_t_|_t_r_u_n_c_a_t_e_c_h_a_r_s_: _o_b_j_._u_s_e_r_|_d_e_f_a_u_l_t_: _e_n
+_"_d_/_m_/_Y_ _H_:_i_:_s_"   _"_d_/_m_/_Y_ _H_:_i_:_s_" _1_0_0_ _}_}                  _"_"_ _}_}             _f_a_v_o_r_i_t_o_s
+_}_}              _}_}
 {% endblock %}
```

## Comparing `django_sh-1.0.8.dist-info/METADATA` & `django_sh-1.0.9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sh
-Version: 1.0.8
+Version: 1.0.9
 Summary: Django shell app for browser
 Home-page: https://gitlab.com/jahazieldom/django-sh
 Author: admintotal-dev
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: django (>=1.8) ; python_version >= "3"
```

## Comparing `django_sh-1.0.8.dist-info/RECORD` & `django_sh-1.0.9.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 django_sh/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_sh/asgi.py,sha256=5DMESr8uSfeJk46cqhsR-fJ6Ie0jA3pfV0d0AL9-UcM,395
 django_sh/settings.py,sha256=Enqdgp7AFuJ3pl9ZsCawFH4Htoa7HV7e0MSrqdlmPMA,3281
 django_sh/urls.py,sha256=nl34DvBEDcDPDtI_0BcqpJLrlWL71CRRbSsGrDKy-SI,797
 django_sh/wsgi.py,sha256=ra87VBevuHsOd9Dx6AITzZGueAzIzVGSY61H-zYN1Vs,395
-sh/__init__.py,sha256=461TEGCGhODEMSQnd42VzO_rSlCsVarBxr01Gx1zUjU,58
+sh/__init__.py,sha256=zU_GE0N2FgCA4QNuDGlDVYzJUBpOUqlnXTwmHLcs6L4,58
 sh/admin.py,sha256=suMo4x8I3JBxAFBVIdE-5qnqZ6JAZV0FESABHOSc-vg,63
 sh/apps.py,sha256=UB18xbXPDYUofP4Ct-8_wDnHOgjCLMdkAmIo_LG4Ek0,79
 sh/models.py,sha256=TAuS1c4AIDjeYEmS3FN5REuQiWPbKc4VeH7Lo3C9nOk,1189
 sh/tests.py,sha256=mrbGGRNg5jwbTJtWWa7zSKdDyeB4vmgZCRc2nk6VY-g,60
 sh/urls.py,sha256=FjCrJI4aK5Giy46Fjtsp7TKMyHwzu6WEgT0f6C3EltQ,715
 sh/views.py,sha256=Yq5SF3SKsvab7fNCIvv2kp3ajkgTJht5sGl2GQAczas,3583
 sh/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -607,15 +607,15 @@
 sh/static/sh/codemirror/theme/vibrant-ink.css,sha256=YeqS2tHXEEKY2-dJ2KAvqX6ovcFhbmblz3ALjsCGLJ0,2142
 sh/static/sh/codemirror/theme/xq-dark.css,sha256=ysjoXXYVnEW2Y_IpzAcFfiibzZ7aQvfH6citOV1-jHQ,3033
 sh/static/sh/codemirror/theme/xq-light.css,sha256=KWl1QR5Q0aRIVE3Y0JUD4B6h48uRxo9QcYLCA4swLTk,2255
 sh/static/sh/codemirror/theme/yeti.css,sha256=8Fi_poAY9nuNFlq0IER8nJnvWJvgjdD-QppK23qtHwc,1884
 sh/static/sh/codemirror/theme/yonce.css,sha256=MCcQDdOHKQzE-fzPAgP6X6A13AIapmGCrrdVrAW84eQ,3075
 sh/static/sh/codemirror/theme/zenburn.css,sha256=nk2UGn3FAu69uhBNqooRdxlVQ7iuCgSPveuh3PbX4Jc,2001
 sh/templates/sh/command.html,sha256=hId2Jz6DJIJHKXb3ULQGq-DCAMEDacTb9KT6Ongke_4,2630
-sh/templates/sh/command_history.html,sha256=7qzWTWc67Ore1IIPzxTHwr_Im17Adcfl4Rp6C7g6JSM,1367
+sh/templates/sh/command_history.html,sha256=VYESaqaIIvGukIKKAqkVkebcWVjhmMZz67rqzYmt26w,1405
 sh/templates/sh/layout.html,sha256=SnjHO1DB5Q5jv7N6UiuAJ_qclv30BU0HC2RY4BC4DPA,3039
 sh/templates/sh/saved_commands.html,sha256=NTe3y1SEo8ZhShzF3KUgIaqZkZpH8fXbo9w_wGPhvu4,1154
 sh/templates/sh/settings.html,sha256=OI-CrNRiuClJpFkleNxATq34-5vd2c7QEAeSy1CdzeI,2339
-django_sh-1.0.8.dist-info/METADATA,sha256=-IUvYbhPS-GIq_IoxOPAuLkB4n7wgW3QxI4-McF0Vi4,645
-django_sh-1.0.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-django_sh-1.0.8.dist-info/top_level.txt,sha256=pTZz3uzb0ffHxcW9uA39Z9eOwVLCZRASpgBVMmiUGxI,13
-django_sh-1.0.8.dist-info/RECORD,,
+django_sh-1.0.9.dist-info/METADATA,sha256=iBCiFAcx4NgdLtJmQpyi62l6srgrsXvw1agLJ7YfCOM,645
+django_sh-1.0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+django_sh-1.0.9.dist-info/top_level.txt,sha256=pTZz3uzb0ffHxcW9uA39Z9eOwVLCZRASpgBVMmiUGxI,13
+django_sh-1.0.9.dist-info/RECORD,,
```

