###Septima module: spatialsuite-aws4


Insert this into your profile themegroups element:

```xml

[if: ModuleDefined("spatialsuite-aws4") ]
<include src="[module:spatialsuite-aws4.dir]/profiles/profile.xml" nodes="/profile/themegroups/*" mustexist="false"/>
[endif]

```

Insert this into your profile themes element:

```xml

[if: ModuleDefined("spatialsuite-aws4") ]
<include src="[module:spatialsuite-aws4.dir]/profiles/profile.xml" nodes="/profile/themes/*" mustexist="false"/>
[endif]
```

Insert this into your targetsetfile:

```xml

[if: ModuleDefined("spatialsuite-aws4") ]
<include src="[module:spatialsuite-aws4.dir]/queries/targetset.xml" nodes="/targetsets/targetset/*" mustexist="true"/>
[endif]

```

