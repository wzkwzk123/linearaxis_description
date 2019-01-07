# linearaxis_description

contains two different sizes of linearaxes: long (Electrolux) and short (Aurora)

### Launch


```
roslaunch linearaxis_description display.launch
```

### switch between models:

for long version:


```
<!-- Import long Axis -->
<xacro:include filename="$(find linearaxis_description)/urdf/linearaxis.macro.xacro" ns="la"/>

<!--Axis Position-->
<xacro:la.axis prefix="linear" parent="base_link" size="long">
<origin xyz="0 0 0" rpy="0 0 0"/>
</xacro:la.axis>
```

for short version (placeholder for now):

```
<!-- Import short Axis -->
<xacro:include filename="$(find linearaxis_description)/urdf/linearaxis.macro.xacro" ns="la"/>

<!--Axis Position-->
<xacro:la.axis prefix="linear" parent="base_link" size="short">
<origin xyz="0 0 0" rpy="0 0 0"/>
</xacro:la.axis>
```