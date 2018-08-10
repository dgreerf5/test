.. role:: raw-latex(raw)
   :format: latex
..

.. raw:: html

   <html xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:w="urn:schemas-microsoft-com:office:word" xmlns:dt="uuid:C2F41010-65B3-11d1-A29F-00AA00C14882" xmlns:m="http://schemas.microsoft.com/office/2004/12/omml" xmlns="http://www.w3.org/TR/REC-html40">

.. raw:: html

   <head>

.. raw:: html

   <title>

BIG-IP Application Security Manager (ASM) Short Coures

.. raw:: html

   </title>

.. raw:: html

   <!--[if gte mso 9]><xml>
    <o:DocumentProperties>
     <o:Author>tsears;lrasmussen</o:Author>
     <o:LastAuthor>Dan Greer</o:LastAuthor>
     <o:Revision>2</o:Revision>
     <o:TotalTime>18</o:TotalTime>
     <o:LastPrinted>2016-07-25T18:18:00Z</o:LastPrinted>
     <o:Created>2018-08-10T16:27:00Z</o:Created>
     <o:LastSaved>2018-08-10T16:27:00Z</o:LastSaved>
     <o:Pages>59</o:Pages>
     <o:Words>8238</o:Words>
     <o:Characters>46957</o:Characters>
     <o:Company>F5 Networks</o:Company>
     <o:Lines>391</o:Lines>
     <o:Paragraphs>110</o:Paragraphs>
     <o:CharactersWithSpaces>55085</o:CharactersWithSpaces>
     <o:Version>16.00</o:Version>
    </o:DocumentProperties>
    <o:CustomDocumentProperties>
     <o:Offisync_UniqueId dt:dt="string">40493</o:Offisync_UniqueId>
     <o:Offisync_ServerID dt:dt="string">a7ce21b1-b0ad-4a12-a7c7-82490448801f</o:Offisync_ServerID>
     <o:Jive_LatestUserAccountName dt:dt="string">greer</o:Jive_LatestUserAccountName>
     <o:Offisync_UpdateToken dt:dt="string">1</o:Offisync_UpdateToken>
     <o:Jive_VersionGuid dt:dt="string">6eff1ca7-8128-47d3-889d-05ba33e32e73</o:Jive_VersionGuid>
     <o:Offisync_ProviderInitializationData dt:dt="string">https://hive.f5.com</o:Offisync_ProviderInitializationData>
     <o:Jive_ModifiedButNotPublished dt:dt="string"></o:Jive_ModifiedButNotPublished>
     <o:Jive_PrevVersionNumber dt:dt="string"></o:Jive_PrevVersionNumber>
     <o:Jive_VersionGuid_v2.5 dt:dt="string"></o:Jive_VersionGuid_v2.5>
     <o:Jive_LatestFileFullName dt:dt="string"></o:Jive_LatestFileFullName>
    </o:CustomDocumentProperties>
    <o:OfficeDocumentSettings>
     <o:RelyOnVML/>
     <o:AllowPNG/>
    </o:OfficeDocumentSettings>
   </xml><![endif]-->

.. raw:: html

   <style>
   <!--
    /* Font Definitions */
    @font-face
       {font-family:Wingdings;
       panose-1:5 0 0 0 0 0 0 0 0 0;
       mso-font-charset:2;
       mso-generic-font-family:decorative;
       mso-font-pitch:variable;
       mso-font-signature:0 268435456 0 0 -2147483648 0;}
   @font-face
       {font-family:SimSun;
       panose-1:2 1 6 0 3 1 1 1 1 1;
       mso-font-alt:宋体;
       mso-font-charset:134;
       mso-generic-font-family:auto;
       mso-font-pitch:variable;
       mso-font-signature:3 680460288 22 0 262145 0;}
   @font-face
       {font-family:"Cambria Math";
       panose-1:2 4 5 3 5 4 6 3 2 4;
       mso-font-charset:0;
       mso-generic-font-family:roman;
       mso-font-pitch:variable;
       mso-font-signature:-536870145 1107305727 0 0 415 0;}
   @font-face
       {font-family:Calibri;
       panose-1:2 15 5 2 2 2 4 3 2 4;
       mso-font-charset:0;
       mso-generic-font-family:swiss;
       mso-font-pitch:variable;
       mso-font-signature:-536859905 -1073697537 9 0 511 0;}
   @font-face
       {font-family:Verdana;
       panose-1:2 11 6 4 3 5 4 4 2 4;
       mso-font-charset:0;
       mso-generic-font-family:swiss;
       mso-font-pitch:variable;
       mso-font-signature:-1593833729 1073750107 16 0 415 0;}
   @font-face
       {font-family:Tahoma;
       panose-1:2 11 6 4 3 5 4 4 2 4;
       mso-font-charset:0;
       mso-generic-font-family:swiss;
       mso-font-pitch:variable;
       mso-font-signature:-520081665 -1073717157 41 0 66047 0;}
   @font-face
       {font-family:Cambria;
       panose-1:2 4 5 3 5 4 6 3 2 4;
       mso-font-charset:0;
       mso-generic-font-family:roman;
       mso-font-pitch:variable;
       mso-font-signature:-536870145 1073743103 0 0 415 0;}
   @font-face
       {font-family:"Arial Black";
       panose-1:2 11 10 4 2 1 2 2 2 4;
       mso-font-charset:0;
       mso-generic-font-family:swiss;
       mso-font-pitch:variable;
       mso-font-signature:-1610612049 1073772795 0 0 159 0;}
   @font-face
       {font-family:"\@SimSun";
       panose-1:2 1 6 0 3 1 1 1 1 1;
       mso-font-charset:134;
       mso-generic-font-family:auto;
       mso-font-pitch:variable;
       mso-font-signature:3 680460288 22 0 262145 0;}
    /* Style Definitions */
    p.MsoNormal, li.MsoNormal, div.MsoNormal
       {mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   h1
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Heading 1 Char";
       mso-style-next:"Body Text";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       mso-outline-level:1;
       font-size:22.0pt;
       mso-bidi-font-size:24.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       font-variant:small-caps;
       mso-font-kerning:16.0pt;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   h2
       {mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Heading 2 Char";
       mso-style-next:"Body Text";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:1.0in;
       text-indent:-1.0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       mso-outline-level:2;
       tab-stops:list 1.0in;
       font-size:18.0pt;
       mso-bidi-font-size:16.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   h3
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Heading 3 Char";
       mso-style-next:Normal;
       margin-top:20.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:4.5pt;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       mso-outline-level:3;
       tab-stops:58.5pt;
       border:none;
       mso-border-top-alt:solid windowtext 1.5pt;
       padding:0in;
       mso-padding-alt:1.0pt 0in 0in 0in;
       font-size:14.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   h4
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Heading 4 Char";
       mso-style-next:"Body Text";
       margin-top:8.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:2.0in;
       text-indent:-1.0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       mso-outline-level:4;
       tab-stops:list 2.0in;
       font-size:11.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#336699;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   h5
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Heading 5 Char";
       mso-style-next:Normal;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:3.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       mso-outline-level:5;
       font-size:13.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;
       font-style:italic;}
   h6
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Heading 6 Char";
       mso-style-next:Normal;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:3.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       mso-outline-level:6;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;}
   p.MsoHeading7, li.MsoHeading7, div.MsoHeading7
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Heading 7 Char";
       mso-style-next:Normal;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:3.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       mso-outline-level:7;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoHeading8, li.MsoHeading8, div.MsoHeading8
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Heading 8 Char";
       mso-style-next:Normal;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:3.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       mso-outline-level:8;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-style:italic;}
   p.MsoHeading9, li.MsoHeading9, div.MsoHeading9
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Heading 9 Char";
       mso-style-next:Normal;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:3.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       mso-outline-level:9;
       font-size:11.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex1, li.MsoIndex1, div.MsoIndex1
       {mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:"Body Text";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:12.0pt;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.MsoIndex2, li.MsoIndex2, div.MsoIndex2
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:24.0pt;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex3, li.MsoIndex3, div.MsoIndex3
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.5in;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex4, li.MsoIndex4, div.MsoIndex4
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:48.0pt;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex5, li.MsoIndex5, div.MsoIndex5
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:60.0pt;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex6, li.MsoIndex6, div.MsoIndex6
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:1.0in;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex7, li.MsoIndex7, div.MsoIndex7
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:84.0pt;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex8, li.MsoIndex8, div.MsoIndex8
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:96.0pt;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoIndex9, li.MsoIndex9, div.MsoIndex9
       {mso-style-update:auto;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:1.5in;
       margin-bottom:.0001pt;
       text-indent:-12.0pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoToc1, li.MsoToc1, div.MsoToc1
       {mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:"Body Text";
       margin-top:.25in;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       tab-stops:right dotted 507.1pt;
       font-size:11.0pt;
       mso-bidi-font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       mso-bidi-font-weight:bold;
       mso-no-proof:yes;}
   p.MsoToc2, li.MsoToc2, div.MsoToc2
       {mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:"Body Text";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:12.25pt;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       tab-stops:right dotted 507.1pt;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       mso-no-proof:yes;}
   p.MsoToc3, li.MsoToc3, div.MsoToc3
       {mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:"Body Text";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:24.0pt;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       tab-stops:right dotted 506.9pt;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       font-style:italic;}
   p.MsoToc4, li.MsoToc4, div.MsoToc4
       {mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.5in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;}
   p.MsoToc5, li.MsoToc5, div.MsoToc5
       {mso-style-update:auto;
       mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:48.0pt;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;}
   p.MsoToc6, li.MsoToc6, div.MsoToc6
       {mso-style-update:auto;
       mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:60.0pt;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;}
   p.MsoToc7, li.MsoToc7, div.MsoToc7
       {mso-style-update:auto;
       mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:1.0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;}
   p.MsoToc8, li.MsoToc8, div.MsoToc8
       {mso-style-update:auto;
       mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:84.0pt;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;}
   p.MsoToc9, li.MsoToc9, div.MsoToc9
       {mso-style-priority:39;
       mso-style-unhide:no;
       mso-style-parent:"TOC 1";
       mso-style-next:"Body Text";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:96.0pt;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       tab-stops:right dotted 507.1pt;
       font-size:9.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       text-transform:uppercase;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;
       mso-no-proof:yes;}
   p.MsoCommentText, li.MsoCommentText, div.MsoCommentText
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Comment Text Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoHeader, li.MsoHeader, div.MsoHeader
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Header Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       tab-stops:center 3.0in right 6.0in;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.MsoFooter, li.MsoFooter, div.MsoFooter
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Footer Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       tab-stops:center 3.0in right 6.0in;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.MsoIndexHeading, li.MsoIndexHeading, div.MsoIndexHeading
       {mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:"Index 1";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:.5in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.MsoCaption, li.MsoCaption, div.MsoCaption
       {mso-style-priority:35;
       mso-style-unhide:no;
       mso-style-link:"Caption Char";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#336699;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.MsoCommentReference
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:8.0pt;
       mso-bidi-font-size:8.0pt;
       font-family:"Times New Roman",serif;
       mso-bidi-font-family:"Times New Roman";}
   span.MsoLineNumber
       {mso-style-priority:99;
       mso-style-unhide:no;
       font-family:"Times New Roman",serif;
       mso-bidi-font-family:"Times New Roman";}
   span.MsoPageNumber
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:9.0pt;
       mso-bidi-font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-ascii-font-family:Arial;
       mso-hansi-font-family:Arial;
       mso-bidi-font-family:Arial;
       color:black;
       mso-ansi-language:EN-GB;}
   p.MsoTitle, li.MsoTitle, div.MsoTitle
       {mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Title Char";
       mso-style-next:Normal;
       margin-top:0in;
       margin-right:0in;
       margin-bottom:15.0pt;
       margin-left:0in;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:48.0pt;
       mso-bidi-font-size:26.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:SimSun;
       mso-fareast-theme-font:major-fareast;
       mso-bidi-font-family:"Times New Roman";
       mso-bidi-theme-font:major-bidi;
       color:black;
       mso-themecolor:text1;
       letter-spacing:.25pt;
       mso-font-kerning:14.0pt;
       mso-fareast-language:EN-US;}
   p.MsoTitleCxSpFirst, li.MsoTitleCxSpFirst, div.MsoTitleCxSpFirst
       {mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Title Char";
       mso-style-next:Normal;
       mso-style-type:export-only;
       margin:0in;
       margin-bottom:.0001pt;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:48.0pt;
       mso-bidi-font-size:26.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:SimSun;
       mso-fareast-theme-font:major-fareast;
       mso-bidi-font-family:"Times New Roman";
       mso-bidi-theme-font:major-bidi;
       color:black;
       mso-themecolor:text1;
       letter-spacing:.25pt;
       mso-font-kerning:14.0pt;
       mso-fareast-language:EN-US;}
   p.MsoTitleCxSpMiddle, li.MsoTitleCxSpMiddle, div.MsoTitleCxSpMiddle
       {mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Title Char";
       mso-style-next:Normal;
       mso-style-type:export-only;
       margin:0in;
       margin-bottom:.0001pt;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:48.0pt;
       mso-bidi-font-size:26.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:SimSun;
       mso-fareast-theme-font:major-fareast;
       mso-bidi-font-family:"Times New Roman";
       mso-bidi-theme-font:major-bidi;
       color:black;
       mso-themecolor:text1;
       letter-spacing:.25pt;
       mso-font-kerning:14.0pt;
       mso-fareast-language:EN-US;}
   p.MsoTitleCxSpLast, li.MsoTitleCxSpLast, div.MsoTitleCxSpLast
       {mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Title Char";
       mso-style-next:Normal;
       mso-style-type:export-only;
       margin-top:0in;
       margin-right:0in;
       margin-bottom:15.0pt;
       margin-left:0in;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:48.0pt;
       mso-bidi-font-size:26.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:SimSun;
       mso-fareast-theme-font:major-fareast;
       mso-bidi-font-family:"Times New Roman";
       mso-bidi-theme-font:major-bidi;
       color:black;
       mso-themecolor:text1;
       letter-spacing:.25pt;
       mso-font-kerning:14.0pt;
       mso-fareast-language:EN-US;}
   p.MsoBodyText, li.MsoBodyText, div.MsoBodyText
       {mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-link:"Body Text Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoBodyTextIndent, li.MsoBodyTextIndent, div.MsoBodyTextIndent
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Body Text Indent Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.25in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.MsoNoteHeading, li.MsoNoteHeading, div.MsoNoteHeading
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Body Text";
       mso-style-link:"Note Heading Char";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:40.5pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.MsoBodyTextIndent2, li.MsoBodyTextIndent2, div.MsoBodyTextIndent2
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Body Text Indent 2 Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.5in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.MsoBodyTextIndent3, li.MsoBodyTextIndent3, div.MsoBodyTextIndent3
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Body Text Indent 3 Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.75in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   a:link, span.MsoHyperlink
       {mso-style-priority:99;
       mso-style-unhide:no;
       font-family:"Times New Roman",serif;
       mso-bidi-font-family:"Times New Roman";
       color:blue;
       text-decoration:underline;
       text-underline:single;}
   a:visited, span.MsoHyperlinkFollowed
       {mso-style-priority:99;
       color:purple;
       mso-themecolor:followedhyperlink;
       text-decoration:underline;
       text-underline:single;}
   p.MsoDocumentMap, li.MsoDocumentMap, div.MsoDocumentMap
       {mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Document Map Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       background:navy;
       font-size:8.0pt;
       font-family:"Tahoma",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-margin-top-alt:auto;
       margin-right:0in;
       mso-margin-bottom-alt:auto;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   code
       {mso-style-priority:99;
       mso-style-parent:"";
       font-family:"Courier New";
       mso-ascii-font-family:"Courier New";
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:"Courier New";
       mso-bidi-font-family:"Courier New";}
   p.MsoCommentSubject, li.MsoCommentSubject, div.MsoCommentSubject
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Comment Text";
       mso-style-link:"Comment Subject Char";
       mso-style-next:"Comment Text";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;}
   p.MsoAcetate, li.MsoAcetate, div.MsoAcetate
       {mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-link:"Balloon Text Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:8.0pt;
       font-family:"Tahoma",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   span.MsoPlaceholderText
       {mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       color:gray;}
   p.MsoNoSpacing, li.MsoNoSpacing, div.MsoNoSpacing
       {mso-style-priority:1;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"";
       mso-style-link:"No Spacing Char";
       margin:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:EN-US;}
   p.MsoRMPane, li.MsoRMPane, div.MsoRMPane
       {mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:Calibri;
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoListParagraph, li.MsoListParagraph, div.MsoListParagraph
       {mso-style-priority:34;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.5in;
       margin-bottom:.0001pt;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoListParagraphCxSpFirst, li.MsoListParagraphCxSpFirst, div.MsoListParagraphCxSpFirst
       {mso-style-priority:34;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-type:export-only;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.5in;
       margin-bottom:.0001pt;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoListParagraphCxSpMiddle, li.MsoListParagraphCxSpMiddle, div.MsoListParagraphCxSpMiddle
       {mso-style-priority:34;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-type:export-only;
       margin-top:0in;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.5in;
       margin-bottom:.0001pt;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoListParagraphCxSpLast, li.MsoListParagraphCxSpLast, div.MsoListParagraphCxSpLast
       {mso-style-priority:34;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-type:export-only;
       margin-top:0in;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.5in;
       margin-bottom:.0001pt;
       mso-add-space:auto;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.MsoTocHeading, li.MsoTocHeading, div.MsoTocHeading
       {mso-style-priority:39;
       mso-style-qformat:yes;
       mso-style-parent:"Heading 1";
       mso-style-next:Normal;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       line-height:115%;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       font-size:14.0pt;
       font-family:"Cambria",serif;
       mso-ascii-font-family:Cambria;
       mso-ascii-theme-font:major-latin;
       mso-fareast-font-family:SimSun;
       mso-fareast-theme-font:major-fareast;
       mso-hansi-font-family:Cambria;
       mso-hansi-theme-font:major-latin;
       mso-bidi-font-family:"Times New Roman";
       mso-bidi-theme-font:major-bidi;
       color:#365F91;
       mso-themecolor:accent1;
       mso-themeshade:191;
       mso-fareast-language:EN-US;
       font-weight:bold;}
   span.Heading1Char
       {mso-style-name:"Heading 1 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 1";
       mso-ansi-font-size:22.0pt;
       mso-bidi-font-size:24.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       font-variant:small-caps;
       mso-font-kerning:16.0pt;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.Heading2Char
       {mso-style-name:"Heading 2 Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 2";
       mso-ansi-font-size:18.0pt;
       mso-bidi-font-size:16.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.Heading3Char
       {mso-style-name:"Heading 3 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 3";
       mso-ansi-font-size:14.0pt;
       mso-bidi-font-size:14.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.Heading4Char
       {mso-style-name:"Heading 4 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 4";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Arial",sans-serif;
       mso-ascii-font-family:Arial;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Arial;
       mso-bidi-font-family:Arial;
       color:#336699;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.Heading5Char
       {mso-style-name:"Heading 5 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 5";
       mso-ansi-font-size:13.0pt;
       mso-bidi-font-size:13.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       font-weight:bold;
       font-style:italic;}
   span.Heading6Char
       {mso-style-name:"Heading 6 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 6";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       font-weight:bold;}
   span.Heading7Char
       {mso-style-name:"Heading 7 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 7";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";}
   span.Heading8Char
       {mso-style-name:"Heading 8 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 8";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       font-style:italic;}
   span.Heading9Char
       {mso-style-name:"Heading 9 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Heading 9";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Arial",sans-serif;
       mso-ascii-font-family:Arial;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Arial;
       mso-bidi-font-family:Arial;}
   span.HeaderChar
       {mso-style-name:"Header Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:Header;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   span.FooterChar
       {mso-style-name:"Footer Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:Footer;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   span.BalloonTextChar
       {mso-style-name:"Balloon Text Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Balloon Text";
       mso-ansi-font-size:8.0pt;
       mso-bidi-font-size:8.0pt;
       font-family:"Tahoma",sans-serif;
       mso-ascii-font-family:Tahoma;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Tahoma;
       mso-bidi-font-family:Tahoma;}
   span.NoSpacingChar
       {mso-style-name:"No Spacing Char";
       mso-style-priority:1;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:"No Spacing";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:EN-US;}
   p.GenericSectionHeader, li.GenericSectionHeader, div.GenericSectionHeader
       {mso-style-name:GenericSectionHeader;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"GenericSectionHeader Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.GenericSectionHeaderChar
       {mso-style-name:"GenericSectionHeader Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:GenericSectionHeader;
       mso-ansi-font-size:12.0pt;
       mso-bidi-font-size:12.0pt;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.GenericBody, li.GenericBody, div.GenericBody
       {mso-style-name:GenericBody;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:GenericSectionHeader;
       mso-style-link:"GenericBody Char";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   span.GenericBodyChar
       {mso-style-name:"GenericBody Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"GenericSectionHeader Char";
       mso-style-link:GenericBody;
       mso-ansi-font-size:12.0pt;
       mso-bidi-font-size:12.0pt;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.apple-style-span
       {mso-style-name:apple-style-span;
       mso-style-unhide:no;
       mso-style-parent:"";}
   span.CommentTextChar
       {mso-style-name:"Comment Text Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Comment Text";
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";}
   span.CommentSubjectChar
       {mso-style-name:"Comment Subject Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"Comment Text Char";
       mso-style-link:"Comment Subject";
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       font-weight:bold;}
   p.Task, li.Task, div.Task
       {mso-style-name:Task;
       mso-style-update:auto;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"Body Text";
       mso-style-link:"Task Char";
       margin-top:7.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:.5in;
       mso-pagination:widow-orphan lines-together;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.BodyTextChar
       {mso-style-name:"Body Text Char";
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:"Body Text";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;}
   span.TaskChar
       {mso-style-name:"Task Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:Task;
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;}
   p.NextLevelTopic, li.NextLevelTopic, div.NextLevelTopic
       {mso-style-name:Next_Level_Topic;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:Task;
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:1.25in;
       text-indent:-13.7pt;
       mso-pagination:widow-orphan lines-together;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Questionquestion, li.Questionquestion, div.Questionquestion
       {mso-style-name:Question_question;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"Body Text";
       mso-style-link:"Question_question Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:20.0pt;
       margin-left:.5in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       mso-list:l8 level1 lfo1;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.QuestionquestionChar
       {mso-style-name:"Question_question Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:Question_question;
       mso-ansi-font-size:10.5pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Calibri;
       mso-bidi-language:HE;}
   p.QuestionsHeading, li.QuestionsHeading, div.QuestionsHeading
       {mso-style-name:Questions_Heading;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"Body Text";
       mso-style-link:"Questions_Heading Char";
       margin-top:16.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:81.0pt;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.QuestionsHeadingChar
       {mso-style-name:"Questions_Heading Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:Questions_Heading;
       mso-ansi-font-size:10.5pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Calibri;
       mso-bidi-language:HE;}
   p.TaskExplanation, li.TaskExplanation, div.TaskExplanation
       {mso-style-name:Task_Explanation;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"Body Text";
       mso-style-link:"Task_Explanation Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:12.0pt;
       margin-left:27.35pt;
       mso-pagination:widow-orphan;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.TaskExplanationChar
       {mso-style-name:"Task_Explanation Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:Task_Explanation;
       mso-ansi-font-size:10.5pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Calibri;
       mso-bidi-language:HE;}
   span.WebLink
       {mso-style-name:WebLink;
       mso-style-priority:1;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       color:#275C9D;
       font-weight:bold;
       mso-bidi-font-weight:normal;
       text-decoration:underline;
       text-underline:single;}
   p.TaskGraphic, li.TaskGraphic, div.TaskGraphic
       {mso-style-name:Task_Graphic;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:Task;
       mso-style-link:"Task_Graphic Char";
       mso-style-next:Task;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan lines-together;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       mso-no-proof:yes;}
   span.TaskGraphicChar
       {mso-style-name:"Task_Graphic Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"Task Char";
       mso-style-link:Task_Graphic;
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;
       mso-no-proof:yes;}
   p.TaskBoldText, li.TaskBoldText, div.TaskBoldText
       {mso-style-name:Task_BoldText;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:Task;
       mso-style-link:"Task_BoldText Char";
       margin-top:7.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:1.0in;
       text-indent:-.25in;
       mso-pagination:widow-orphan lines-together;
       mso-list:l14 level1 lfo2;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.TaskBoldTextChar
       {mso-style-name:"Task_BoldText Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"";
       mso-style-link:Task_BoldText;
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.DocumentMapChar
       {mso-style-name:"Document Map Char";
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Document Map";
       mso-ansi-font-size:8.0pt;
       mso-bidi-font-size:8.0pt;
       font-family:"Tahoma",sans-serif;
       mso-ascii-font-family:Tahoma;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Tahoma;
       mso-bidi-font-family:Tahoma;
       background:navy;}
   p.Style1, li.Style1, div.Style1
       {mso-style-name:Style1;
       mso-style-unhide:no;
       mso-style-parent:"Heading 1";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       mso-outline-level:1;
       font-size:22.0pt;
       mso-bidi-font-size:24.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       font-variant:small-caps;
       mso-font-kerning:16.0pt;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       font-style:italic;
       mso-bidi-font-style:normal;}
   p.Style2, li.Style2, div.Style2
       {mso-style-name:Style2;
       mso-style-update:auto;
       mso-style-unhide:no;
       mso-style-parent:"Heading 1";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       mso-outline-level:1;
       font-size:22.0pt;
       mso-bidi-font-size:24.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       font-variant:small-caps;
       mso-font-kerning:16.0pt;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       font-style:italic;
       mso-bidi-font-style:normal;}
   p.StyleHeading212pt, li.StyleHeading212pt, div.StyleHeading212pt
       {mso-style-name:"Style Heading 2 + 12 pt";
       mso-style-update:auto;
       mso-style-unhide:no;
       mso-style-parent:"Heading 2";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       mso-outline-level:2;
       font-size:12.0pt;
       mso-bidi-font-size:14.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       font-style:italic;}
   span.htmlval1
       {mso-style-name:html_val1;
       mso-style-unhide:no;
       mso-style-parent:"";
       color:blue;}
   span.amdocs
       {mso-style-name:amdocs;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:16.0pt;
       mso-bidi-font-size:16.0pt;
       font-family:"Arial",sans-serif;
       mso-ascii-font-family:Arial;
       mso-hansi-font-family:Arial;
       mso-bidi-font-family:Arial;
       color:windowtext;
       text-decoration:none;
       text-underline:none;}
   span.app
       {mso-style-name:app;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:16.0pt;
       mso-bidi-font-size:16.0pt;
       font-family:"Arial Black",sans-serif;
       mso-ascii-font-family:"Arial Black";
       mso-hansi-font-family:"Arial Black";
       mso-bidi-font-family:"Times New Roman";
       color:red;}
   p.AppNameNot, li.AppNameNot, div.AppNameNot
       {mso-style-name:"App Name Not";
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       margin-top:40.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:36.0pt;
       mso-bidi-font-size:28.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       font-weight:bold;
       mso-no-proof:yes;}
   p.AppendixHeading1, li.AppendixHeading1, div.AppendixHeading1
       {mso-style-name:"Appendix Heading1";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:40.0pt;
       margin-right:0in;
       margin-bottom:12.0pt;
       margin-left:2.1in;
       text-indent:-2.1in;
       mso-pagination:widow-orphan;
       mso-outline-level:1;
       tab-stops:2.1in;
       border:none;
       mso-border-bottom-alt:solid windowtext .5pt;
       padding:0in;
       mso-padding-alt:0in 0in 1.0pt 0in;
       font-size:24.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#FF6600;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.AppendixHeading2, li.AppendixHeading2, div.AppendixHeading2
       {mso-style-name:"Appendix Heading2";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:84.0pt;
       text-indent:-1.0in;
       mso-pagination:widow-orphan lines-together;
       mso-outline-level:2;
       tab-stops:1.0in list 84.0pt;
       font-size:16.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.AppendixHeading3, li.AppendixHeading3, div.AppendixHeading3
       {mso-style-name:"Appendix Heading3";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:8.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:120.0pt;
       text-indent:-1.0in;
       mso-pagination:widow-orphan;
       mso-outline-level:3;
       tab-stops:1.5in list 120.0pt;
       font-size:14.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#336699;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.AppendixHeading4, li.AppendixHeading4, div.AppendixHeading4
       {mso-style-name:"Appendix Heading4";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:156.0pt;
       margin-bottom:.0001pt;
       text-indent:-1.0in;
       mso-pagination:widow-orphan;
       mso-outline-level:4;
       tab-stops:2.0in list 156.0pt;
       font-size:11.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#336699;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.BodyTextIndentChar
       {mso-style-name:"Body Text Indent Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Body Text Indent";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   span.BodyTextIndent2Char
       {mso-style-name:"Body Text Indent 2 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Body Text Indent 2";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   p.BodyTextIndent2Table, li.BodyTextIndent2Table, div.BodyTextIndent2Table
       {mso-style-name:"Body Text Indent 2 Table";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.5in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.BodyTextIndent3Char
       {mso-style-name:"Body Text Indent 3 Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Body Text Indent 3";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   p.BodyTextIndent3Table, li.BodyTextIndent3Table, div.BodyTextIndent3Table
       {mso-style-name:"Body Text Indent 3 Table";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:54.7pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.BodyTextIndentTable, li.BodyTextIndentTable, div.BodyTextIndentTable
       {mso-style-name:"Body Text Indent Table";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.3in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.BodyText, li.BodyText, div.BodyText
       {mso-style-name:BodyText;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:"Body Text";
       mso-style-link:"BodyText Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.5in;
       mso-pagination:widow-orphan;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.BodyTextChar0
       {mso-style-name:"BodyText Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:BodyText;
       mso-ansi-font-size:10.5pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;}
   p.Bullet1square, li.Bullet1square, div.Bullet1square
       {mso-style-name:"Bullet 1 \(square\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.25in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list 1.25in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Bullet2round, li.Bullet2round, div.Bullet2round
       {mso-style-name:"Bullet 2 \(round\)";
       mso-style-noshow:yes;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.5in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list 1.5in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Bullet3hollow, li.Bullet3hollow, div.Bullet3hollow
       {mso-style-name:"Bullet 3 \(hollow\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.75in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list 1.75in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Bullet1subtitle, li.Bullet1subtitle, div.Bullet1subtitle
       {mso-style-name:"Bullet1 subtitle";
       mso-style-update:auto;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.15in;
       text-indent:-.15in;
       mso-pagination:widow-orphan;
       tab-stops:list 0in left .25in;
       font-size:12.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.BulletedPoints, li.BulletedPoints, div.BulletedPoints
       {mso-style-name:"Bulleted Points";
       mso-style-unhide:no;
       mso-style-qformat:yes;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:.75in;
       text-indent:-.25in;
       line-height:115%;
       mso-pagination:widow-orphan;
       mso-list:l4 level1 lfo34;
       font-size:11.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:EN-US;}
   p.CallOut, li.CallOut, div.CallOut
       {mso-style-name:CallOut;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:BodyText;
       mso-style-link:"CallOut Char";
       margin-top:9.0pt;
       margin-right:1.05in;
       margin-bottom:9.0pt;
       margin-left:.75in;
       text-indent:-.6in;
       mso-pagination:widow-orphan;
       background:#FDE9D9;
       mso-background-themecolor:accent6;
       mso-background-themetint:51;
       border:none;
       mso-border-alt:solid windowtext .5pt;
       padding:0in;
       mso-padding-alt:1.0pt 4.0pt 1.0pt 4.0pt;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       background:#FDE9D9;
       mso-shading-themecolor:accent6;
       mso-shading-themetint:51;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.CallOutChar
       {mso-style-name:"CallOut Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"BodyText Char";
       mso-style-link:CallOut;
       mso-ansi-font-size:10.5pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       background:#FDE9D9;
       mso-shading-themecolor:accent6;
       mso-shading-themetint:51;
       mso-bidi-language:HE;}
   span.CaptionChar
       {mso-style-name:"Caption Char";
       mso-style-priority:35;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:Caption;
       font-family:"Arial",sans-serif;
       mso-ascii-font-family:Arial;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Arial;
       mso-bidi-font-family:Arial;
       color:#336699;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.Code, li.Code, div.Code
       {mso-style-name:Code;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Courier New";
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       mso-no-proof:yes;}
   span.Command
       {mso-style-name:Command;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:10.0pt;
       mso-bidi-font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-ascii-font-family:Arial;
       mso-hansi-font-family:Arial;
       mso-bidi-font-family:Arial;
       font-weight:bold;}
   p.CommandPromptText, li.CommandPromptText, div.CommandPromptText
       {mso-style-name:"Command Prompt Text";
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"Command Prompt Text Char";
       mso-style-next:Task;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:76.3pt;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       mso-bidi-font-size:9.5pt;
       font-family:"Courier New";
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.CommandPromptTextChar
       {mso-style-name:"Command Prompt Text Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Command Prompt Text";
       mso-ansi-font-size:9.0pt;
       mso-bidi-font-size:9.5pt;
       font-family:"Courier New";
       mso-ascii-font-family:"Courier New";
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:"Courier New";
       mso-bidi-font-family:"Courier New";
       mso-bidi-language:HE;}
   p.ConfidentialInformation, li.ConfidentialInformation, div.ConfidentialInformation
       {mso-style-name:"Confidential Information";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Contents, li.Contents, div.Contents
       {mso-style-name:Contents;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:40.0pt;
       margin-right:0in;
       margin-bottom:24.0pt;
       margin-left:0in;
       text-align:center;
       mso-pagination:widow-orphan;
       mso-outline-level:1;
       font-size:20.0pt;
       mso-bidi-font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.Definitions, li.Definitions, div.Definitions
       {mso-style-name:Definitions;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.DocumentInformation, li.DocumentInformation, div.DocumentInformation
       {mso-style-name:"Document Information";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:12.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.DocumentType, li.DocumentType, div.DocumentType
       {mso-style-name:"Document Type";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:20.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:26.0pt;
       mso-bidi-font-size:24.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Exercise2, li.Exercise2, div.Exercise2
       {mso-style-name:Exercise2;
       mso-style-update:auto;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Heading 2";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:102.25pt;
       text-indent:-62.65pt;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       mso-outline-level:2;
       tab-stops:list 102.0pt;
       font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Exercise3, li.Exercise3, div.Exercise3
       {mso-style-name:Exercise3;
       mso-style-update:auto;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Heading 3";
       margin-top:20.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       mso-outline-level:3;
       tab-stops:58.5pt;
       border:none;
       mso-border-top-alt:solid windowtext 1.5pt;
       padding:0in;
       mso-padding-alt:1.0pt 0in 0in 0in;
       font-size:12.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Figure, li.Figure, div.Figure
       {mso-style-name:Figure;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.FirstFooter, li.FirstFooter, div.FirstFooter
       {mso-style-name:"First Footer";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:Footer;
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:0in;
       text-align:right;
       mso-pagination:widow-orphan lines-together;
       tab-stops:center 3.0in;
       font-size:9.0pt;
       mso-bidi-font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.FooterEven, li.FooterEven, div.FooterEven
       {mso-style-name:"Footer Even";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:Footer;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan lines-together;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.FooterFirst, li.FooterFirst, div.FooterFirst
       {mso-style-name:"Footer First";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin:0in;
       margin-bottom:.0001pt;
       text-align:right;
       mso-pagination:widow-orphan lines-together;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.FooterLandscape, li.FooterLandscape, div.FooterLandscape
       {mso-style-name:"Footer Landscape";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan lines-together;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.FooterOdd, li.FooterOdd, div.FooterOdd
       {mso-style-name:"Footer Odd";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:Footer;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       text-align:right;
       mso-pagination:widow-orphan lines-together;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.FooterPortrait, li.FooterPortrait, div.FooterPortrait
       {mso-style-name:"Footer Portrait";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin:0in;
       margin-bottom:.0001pt;
       text-align:right;
       mso-pagination:widow-orphan lines-together;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.HeaderEven, li.HeaderEven, div.HeaderEven
       {mso-style-name:"Header Even";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:Header;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       border:none;
       mso-border-bottom-alt:solid windowtext 1.0pt;
       padding:0in;
       mso-padding-alt:0in 0in 1.0pt 0in;
       font-size:9.0pt;
       font-family:"Verdana",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Arial;
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.HeaderLandscape, li.HeaderLandscape, div.HeaderLandscape
       {mso-style-name:"Header Landscape";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       border:none;
       mso-border-bottom-alt:solid windowtext 1.0pt;
       padding:0in;
       mso-padding-alt:0in 0in 1.0pt 0in;
       font-size:9.0pt;
       font-family:"Verdana",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Arial;
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.HeaderOdd, li.HeaderOdd, div.HeaderOdd
       {mso-style-name:"Header Odd";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin:0in;
       margin-bottom:.0001pt;
       text-align:right;
       mso-pagination:widow-orphan;
       border:none;
       mso-border-bottom-alt:solid windowtext 1.0pt;
       padding:0in;
       mso-padding-alt:0in 0in 1.0pt 0in;
       font-size:9.0pt;
       font-family:"Verdana",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Arial;
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.HeaderPortrait, li.HeaderPortrait, div.HeaderPortrait
       {mso-style-name:"Header Portrait";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-link:"Header Portrait Char";
       margin:0in;
       margin-bottom:.0001pt;
       text-align:right;
       mso-pagination:widow-orphan;
       border:none;
       mso-border-bottom-alt:solid windowtext 1.0pt;
       padding:0in;
       mso-padding-alt:0in 0in 1.0pt 0in;
       font-size:9.0pt;
       font-family:"Verdana",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:Arial;
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.HeaderPortraitChar
       {mso-style-name:"Header Portrait Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Header Portrait";
       mso-ansi-font-size:9.0pt;
       mso-bidi-font-size:9.0pt;
       font-family:"Verdana",sans-serif;
       mso-ascii-font-family:Verdana;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Verdana;
       mso-bidi-font-family:Arial;
       color:#003366;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.Heading3-First, li.Heading3-First, div.Heading3-First
       {mso-style-name:"Heading 3 - First";
       mso-style-unhide:no;
       mso-style-parent:"Heading 3";
       mso-style-link:"Heading 3 - First Char";
       margin-top:20.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:22.5pt;
       text-indent:-.25in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       mso-outline-level:3;
       tab-stops:58.5pt;
       border:none;
       mso-border-top-alt:solid windowtext 1.5pt;
       padding:0in;
       mso-padding-alt:1.0pt 0in 0in 0in;
       font-size:14.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.Heading3-FirstChar
       {mso-style-name:"Heading 3 - First Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"Heading 3 Char";
       mso-style-link:"Heading 3 - First";
       mso-ansi-font-size:14.0pt;
       mso-bidi-font-size:14.0pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.IndexTitle, li.IndexTitle, div.IndexTitle
       {mso-style-name:"Index Title";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Index 1";
       margin-top:40.0pt;
       margin-right:0in;
       margin-bottom:12.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       mso-outline-level:1;
       border:none;
       mso-border-bottom-alt:solid windowtext .5pt;
       padding:0in;
       mso-padding-alt:0in 0in 1.0pt 0in;
       font-size:24.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       font-variant:small-caps;
       color:#FF6600;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.infotable, li.infotable, div.infotable
       {mso-style-name:infotable;
       mso-style-unhide:no;
       mso-margin-top-alt:auto;
       margin-right:0in;
       mso-margin-bottom-alt:auto;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       mso-bidi-font-size:12.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.LabTaskHdr, li.LabTaskHdr, div.LabTaskHdr
       {mso-style-name:"Lab Task Hdr";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-next:Normal;
       margin-top:6.0pt;
       margin-right:.05in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.Lab, li.Lab, div.Lab
       {mso-style-name:Lab;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Lab Task Hdr";
       margin-top:6.0pt;
       margin-right:.05in;
       margin-bottom:6.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.LabDataList, li.LabDataList, div.LabDataList
       {mso-style-name:"Lab Data List";
       mso-style-priority:99;
       mso-style-unhide:no;
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:.25in;
       margin-bottom:.0001pt;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       mso-list:l17 level1 lfo35;
       tab-stops:list .25in;
       font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   p.Objective, li.Objective, div.Objective
       {mso-style-name:Objective;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-next:"Bulleted Points";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:14.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.LabReq, li.LabReq, div.LabReq
       {mso-style-name:"Lab Req";
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:Objective;
       mso-style-next:"Bulleted Points";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:14.0pt;
       font-family:"Calibri",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.LabTask, li.LabTask, div.LabTask
       {mso-style-name:"Lab Task";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Body Text";
       margin-top:6.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:.25in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list .25in;
       font-size:10.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.List1number, li.List1number, div.List1number
       {mso-style-name:"List 1 \(number\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.25in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list 1.25in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.List2alpha, li.List2alpha, div.List2alpha
       {mso-style-name:"List 2 \(alpha\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.5in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list 107.3pt;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.List3roman, li.List3roman, div.List3roman
       {mso-style-name:"List 3 \(roman\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:0in;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.75in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:1.75in list 2.0in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.List-intro, li.List-intro, div.List-intro
       {mso-style-name:List-intro;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.name1
       {mso-style-name:name1;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:16.0pt;
       mso-bidi-font-size:16.0pt;
       font-family:"Arial Black",sans-serif;
       mso-ascii-font-family:"Arial Black";
       mso-hansi-font-family:"Arial Black";
       mso-bidi-font-family:Arial;
       color:black;}
   span.name2
       {mso-style-name:name2;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-ansi-font-size:16.0pt;
       font-family:"Arial Black",sans-serif;
       mso-ascii-font-family:"Arial Black";
       mso-hansi-font-family:"Arial Black";
       mso-bidi-font-family:"Times New Roman";
       color:red;}
   p.Note, li.Note, div.Note
       {mso-style-name:Note;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.75in;
       text-indent:-.5in;
       mso-pagination:widow-orphan;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-style:italic;}
   span.NoteHeadingChar
       {mso-style-name:"Note Heading Char";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:"Note Heading";
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   p.NoteIcon, li.NoteIcon, div.NoteIcon
       {mso-style-name:"Note Icon";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:2.0in;
       mso-pagination:widow-orphan;
       tab-stops:161.0pt;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Profile, li.Profile, div.Profile
       {mso-style-name:Profile;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.ProfileField, li.ProfileField, div.ProfileField
       {mso-style-name:"Profile Field";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:0in;
       margin-left:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.TableHeader, li.TableHeader, div.TableHeader
       {mso-style-name:"Table Header";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:2.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.ReleaseNotesHeader, li.ReleaseNotesHeader, div.ReleaseNotesHeader
       {mso-style-name:"ReleaseNotes Header";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"Table Header";
       margin-top:2.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       font-size:9.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       color:#003366;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.ReleaseNotesTitle, li.ReleaseNotesTitle, div.ReleaseNotesTitle
       {mso-style-name:"ReleaseNotes Title";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:12.0pt;
       margin-left:0in;
       text-align:center;
       mso-pagination:widow-orphan;
       font-size:14.0pt;
       font-family:"Arial",sans-serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.Step, li.Step, div.Step
       {mso-style-name:Step;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.25in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list .75in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.SubStep, li.SubStep, div.SubStep
       {mso-style-name:SubStep;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.5in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list 1.0in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TableBody, li.TableBody, div.TableBody
       {mso-style-name:"Table Body";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:2.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:0in;
       mso-pagination:widow-orphan lines-together;
       page-break-after:avoid;
       font-size:10.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TableList1number, li.TableList1number, div.TableList1number
       {mso-style-name:"Table List 1 \(number\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.25in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list .25in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TableList2alpha, li.TableList2alpha, div.TableList2alpha
       {mso-style-name:"Table List 2 \(alpha\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.5in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:list .5in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TableList3roman, li.TableList3roman, div.TableList3roman
       {mso-style-name:"Table List 3 \(roman\)";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.75in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       tab-stops:.75in list 1.0in;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.Tablepostpara, li.Tablepostpara, div.Tablepostpara
       {mso-style-name:"Table post para";
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TableEntry, li.TableEntry, div.TableEntry
       {mso-style-name:Table_Entry;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-link:"Table_Entry Char";
       margin:0in;
       margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.TableEntryChar
       {mso-style-name:"Table_Entry Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:Table_Entry;
       mso-ansi-font-size:11.0pt;
       mso-bidi-font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-ascii-font-family:"Times New Roman";
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:"Times New Roman";
       mso-bidi-language:HE;}
   p.TaskNote, li.TaskNote, div.TaskNote
       {mso-style-name:"Task Note";
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:Task;
       margin-top:7.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:59.05pt;
       text-indent:-13.7pt;
       mso-pagination:widow-orphan lines-together;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   p.TaskStart, li.TaskStart, div.TaskStart
       {mso-style-name:"Task Start";
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-parent:Task;
       margin-top:12.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:27.35pt;
       mso-pagination:widow-orphan lines-together;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TemplateCode, li.TemplateCode, div.TemplateCode
       {mso-style-name:Template_Code;
       mso-style-unhide:no;
       mso-style-parent:Task;
       mso-style-link:"Template_Code Char";
       margin-top:2.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:49.7pt;
       mso-pagination:widow-orphan lines-together;
       font-size:9.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Courier New";
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   span.TemplateCodeChar
       {mso-style-name:"Template_Code Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-parent:"Task Char";
       mso-style-link:Template_Code;
       mso-ansi-font-size:9.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Courier New";
       mso-ascii-font-family:"Courier New";
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:"Courier New";
       mso-bidi-font-family:"Courier New";
       mso-bidi-language:HE;}
   p.Terms, li.Terms, div.Terms
       {mso-style-name:Terms;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   span.TitleChar
       {mso-style-name:"Title Char";
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:Title;
       mso-ansi-font-size:48.0pt;
       mso-bidi-font-size:26.0pt;
       font-family:SimSun;
       mso-fareast-font-family:SimSun;
       mso-fareast-theme-font:major-fareast;
       mso-bidi-font-family:"Times New Roman";
       mso-bidi-theme-font:major-bidi;
       color:black;
       mso-themecolor:text1;
       letter-spacing:.25pt;
       mso-font-kerning:14.0pt;}
   p.ToDo, li.ToDo, div.ToDo
       {mso-style-name:ToDo;
       mso-style-priority:99;
       mso-style-unhide:no;
       mso-style-parent:"";
       mso-style-next:"Body Text";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:1.0in;
       mso-pagination:widow-orphan;
       page-break-after:avoid;
       font-size:11.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;}
   p.TopLevelTask, li.TopLevelTask, div.TopLevelTask
       {mso-style-name:Top_Level_Task;
       mso-style-noshow:yes;
       mso-style-unhide:no;
       mso-style-parent:Task;
       margin-top:7.0pt;
       margin-right:0in;
       margin-bottom:2.0pt;
       margin-left:.5in;
       mso-pagination:widow-orphan lines-together;
       font-size:11.0pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.TopLevelTopic, li.TopLevelTopic, div.TopLevelTopic
       {mso-style-name:Top_Level_Topic;
       mso-style-noshow:yes;
       mso-style-unhide:no;
       mso-style-parent:BodyText;
       mso-style-next:Normal;
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:4.0pt;
       margin-left:.75in;
       text-indent:-.25in;
       mso-pagination:widow-orphan;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;}
   p.WhichPartner, li.WhichPartner, div.WhichPartner
       {mso-style-name:WhichPartner;
       mso-style-noshow:yes;
       mso-style-unhide:no;
       mso-style-qformat:yes;
       mso-style-link:"WhichPartner Char";
       margin-top:4.0pt;
       margin-right:0in;
       margin-bottom:6.0pt;
       margin-left:27.35pt;
       mso-pagination:widow-orphan;
       font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-fareast-language:EN-US;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.WhichPartnerChar
       {mso-style-name:"WhichPartner Char";
       mso-style-noshow:yes;
       mso-style-unhide:no;
       mso-style-locked:yes;
       mso-style-link:WhichPartner;
       mso-ansi-font-size:10.5pt;
       mso-bidi-font-size:10.5pt;
       font-family:"Calibri",sans-serif;
       mso-ascii-font-family:Calibri;
       mso-ascii-theme-font:minor-latin;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Calibri;
       mso-hansi-theme-font:minor-latin;
       mso-bidi-font-family:Calibri;
       mso-bidi-theme-font:minor-latin;
       mso-bidi-language:HE;
       font-weight:bold;
       mso-bidi-font-weight:normal;}
   span.SpellE
       {mso-style-name:"";
       mso-spl-e:yes;}
   span.GramE
       {mso-style-name:"";
       mso-gram-e:yes;}
   .MsoChpDefault
       {mso-style-type:export-only;
       mso-default-props:yes;
       font-size:10.0pt;
       mso-ansi-font-size:10.0pt;
       mso-bidi-font-size:10.0pt;
       mso-ascii-font-family:Calibri;
       mso-fareast-font-family:Calibri;
       mso-hansi-font-family:Calibri;
       mso-fareast-language:EN-US;}
    /* Page Definitions */
    @page
       {mso-footnote-separator:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") fs;
       mso-footnote-continuation-separator:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") fcs;
       mso-endnote-separator:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") es;
       mso-endnote-continuation-separator:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") ecs;}
   @page WordSection1
       {size:8.5in 11.0in;
       margin:1.0in .6in .5in .6in;
       mso-header-margin:.7in;
       mso-footer-margin:.7in;
       mso-gutter-margin:.25in;
       mso-title-page:yes;
       mso-even-header:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") eh1;
       mso-even-footer:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") ef1;
       mso-footer:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") f1;
       mso-paper-source:0;}
   div.WordSection1
       {page:WordSection1;}
   @page WordSection2
       {size:8.5in 11.0in;
       margin:.5in .5in .5in .5in;
       mso-header-margin:.3in;
       mso-footer-margin:.3in;
       mso-even-header:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") eh2;
       mso-header:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") h2;
       mso-even-footer:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") ef2;
       mso-footer:url("LTM%20Fundamentals%20v13.1%20Lab.fld/header.html") f2;
       mso-paper-source:0;}
   div.WordSection2
       {page:WordSection2;}
    /* List Definitions */
    @list l0
       {mso-list-id:112017807;
       mso-list-type:hybrid;
       mso-list-template-ids:275535248 67698703 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l0:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l0:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l0:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l0:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l0:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l0:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l0:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.75in;
       text-indent:-.25in;}
   @list l0:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:5.25in;
       text-indent:-.25in;}
   @list l0:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:5.75in;
       text-indent:-9.0pt;}
   @list l1
       {mso-list-id:138881389;
       mso-list-type:hybrid;
       mso-list-template-ids:197054340 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l1:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l1:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l1:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l1:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l1:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l1:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l1:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l1:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l1:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l2
       {mso-list-id:188759026;
       mso-list-type:hybrid;
       mso-list-template-ids:-212566672 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l2:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l2:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l2:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l2:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l2:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l2:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l2:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l2:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l2:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l3
       {mso-list-id:233777576;
       mso-list-type:hybrid;
       mso-list-template-ids:434022394 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l3:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l3:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l3:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l3:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l3:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l3:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l3:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l3:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l3:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l4
       {mso-list-id:439836401;
       mso-list-type:hybrid;
       mso-list-template-ids:-24613640 1377354634 67698691 67698693 67698689 67698691 67698693 67698689 67698691 67698693;}
   @list l4:level1
       {mso-level-number-format:bullet;
       mso-level-style-link:"Bulleted Points";
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l4:level2
       {mso-level-number-format:bullet;
       mso-level-text:o;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;
       font-family:"Courier New";}
   @list l4:level3
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;
       font-family:Wingdings;}
   @list l4:level4
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l4:level5
       {mso-level-number-format:bullet;
       mso-level-text:o;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;
       font-family:"Courier New";}
   @list l4:level6
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;
       font-family:Wingdings;}
   @list l4:level7
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l4:level8
       {mso-level-number-format:bullet;
       mso-level-text:o;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;
       font-family:"Courier New";}
   @list l4:level9
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.75in;
       text-indent:-.25in;
       font-family:Wingdings;}
   @list l5
       {mso-list-id:461656104;
       mso-list-type:hybrid;
       mso-list-template-ids:73172036 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l5:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l5:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l5:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l5:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l5:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l5:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l5:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l5:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l5:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l6
       {mso-list-id:508830313;
       mso-list-type:hybrid;
       mso-list-template-ids:608329966 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l6:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l6:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l6:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l6:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l6:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l6:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l6:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l6:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l6:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l7
       {mso-list-id:550844554;
       mso-list-type:hybrid;
       mso-list-template-ids:-1393109098 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l7:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l7:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l7:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l7:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l7:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l7:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l7:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l7:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l7:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l8
       {mso-list-id:603999234;
       mso-list-type:hybrid;
       mso-list-template-ids:-2133302902 1752568628 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l8:level1
       {mso-level-number-format:alpha-lower;
       mso-level-style-link:Question_question;
       mso-level-text:"%1\)";
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l8:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l8:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l8:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l8:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l8:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l8:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.75in;
       text-indent:-.25in;}
   @list l8:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:5.25in;
       text-indent:-.25in;}
   @list l8:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:5.75in;
       text-indent:-9.0pt;}
   @list l9
       {mso-list-id:624779187;
       mso-list-type:hybrid;
       mso-list-template-ids:-1459947712 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l9:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l9:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l9:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l9:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l9:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l9:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l9:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l9:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l9:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l10
       {mso-list-id:655114687;
       mso-list-type:hybrid;
       mso-list-template-ids:-1883312086 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l10:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l10:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l10:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l10:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l10:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l10:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l10:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l10:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l10:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l11
       {mso-list-id:729841529;
       mso-list-template-ids:197054340;
       mso-list-style-priority:99;
       mso-list-style-name:Style3;}
   @list l11:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l11:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l11:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l11:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l11:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l11:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l11:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l11:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l11:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l12
       {mso-list-id:896207177;
       mso-list-type:hybrid;
       mso-list-template-ids:-567240328 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l12:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l12:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l12:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l12:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l12:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l12:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l12:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l12:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l12:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l13
       {mso-list-id:904221091;
       mso-list-type:hybrid;
       mso-list-template-ids:-14378644 1151112610 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l13:level1
       {mso-level-start-at:5;
       mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.0in;
       text-indent:-.25in;}
   @list l13:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.5in;
       text-indent:-.25in;}
   @list l13:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.0in;
       text-indent:-9.0pt;}
   @list l13:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.5in;
       text-indent:-.25in;}
   @list l13:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.0in;
       text-indent:-.25in;}
   @list l13:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.5in;
       text-indent:-9.0pt;}
   @list l13:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.0in;
       text-indent:-.25in;}
   @list l13:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.5in;
       text-indent:-.25in;}
   @list l13:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:5.0in;
       text-indent:-9.0pt;}
   @list l14
       {mso-list-id:920597855;
       mso-list-type:hybrid;
       mso-list-template-ids:-1930164874 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l14:level1
       {mso-level-number-format:alpha-lower;
       mso-level-style-link:Task_BoldText;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l14:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l14:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l14:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l14:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l14:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l14:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l14:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l14:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l15
       {mso-list-id:930894394;
       mso-list-type:hybrid;
       mso-list-template-ids:-1757118966 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l15:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l15:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l15:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l15:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l15:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l15:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l15:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l15:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l15:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l16
       {mso-list-id:968559242;
       mso-list-type:hybrid;
       mso-list-template-ids:35560536 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l16:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l16:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l16:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l16:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l16:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l16:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l16:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l16:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l16:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l17
       {mso-list-id:1064722347;
       mso-list-type:simple;
       mso-list-template-ids:1318471290;}
   @list l17:level1
       {mso-level-number-format:bullet;
       mso-level-style-link:"Lab Data List";
       mso-level-text:;
       mso-level-tab-stop:.25in;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l18
       {mso-list-id:1075279870;
       mso-list-type:hybrid;
       mso-list-template-ids:1395028372 67698715 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l18:level1
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l18:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l18:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l18:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l18:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l18:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l18:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l18:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l18:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l19
       {mso-list-id:1127233967;
       mso-list-type:hybrid;
       mso-list-template-ids:928260388 67698703 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l19:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l19:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l19:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l19:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l19:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l19:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l19:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.75in;
       text-indent:-.25in;}
   @list l19:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:5.25in;
       text-indent:-.25in;}
   @list l19:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:5.75in;
       text-indent:-9.0pt;}
   @list l20
       {mso-list-id:1226836158;
       mso-list-type:hybrid;
       mso-list-template-ids:2041483424 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l20:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l20:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l20:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l20:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l20:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l20:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l20:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l20:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l20:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l21
       {mso-list-id:1456215477;
       mso-list-type:hybrid;
       mso-list-template-ids:-212566672 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l21:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l21:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l21:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l21:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l21:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l21:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l21:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l21:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l21:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l22
       {mso-list-id:1486966318;
       mso-list-type:hybrid;
       mso-list-template-ids:-212566672 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l22:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l22:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l22:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l22:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l22:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l22:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l22:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l22:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l22:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l23
       {mso-list-id:1495759131;
       mso-list-type:hybrid;
       mso-list-template-ids:2041483424 -18850870 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l23:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.25in;
       text-indent:-.25in;}
   @list l23:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l23:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l23:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l23:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l23:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l23:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l23:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l23:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l24
       {mso-list-id:1582567979;
       mso-list-type:hybrid;
       mso-list-template-ids:1681173264 111956076 -1315939454 390236364 -1530634422 -130915766 275396284 524313604 1916058206 1019909144;}
   @list l24:level1
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:.5in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level2
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:1.0in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level3
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:1.5in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level4
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:2.0in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level5
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:2.5in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level6
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:3.0in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level7
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:3.5in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level8
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:4.0in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l24:level9
       {mso-level-number-format:bullet;
       mso-level-text:•;
       mso-level-tab-stop:4.5in;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Arial",sans-serif;
       mso-bidi-font-family:"Times New Roman";}
   @list l25
       {mso-list-id:1634749612;
       mso-list-type:hybrid;
       mso-list-template-ids:1042815250 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l25:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l25:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l25:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l25:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l25:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l25:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l25:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l25:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l25:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l26
       {mso-list-id:1935819272;
       mso-list-type:hybrid;
       mso-list-template-ids:-301837680 67698715 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l26:level1
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l26:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l26:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l26:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l26:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l26:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l26:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l26:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l26:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l27
       {mso-list-id:1938561386;
       mso-list-type:hybrid;
       mso-list-template-ids:1079261066 67698689 67698691 67698693 67698689 67698691 67698693 67698689 67698691 67698693;}
   @list l27:level1
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l27:level2
       {mso-level-number-format:bullet;
       mso-level-text:o;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Courier New";}
   @list l27:level3
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:Wingdings;}
   @list l27:level4
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l27:level5
       {mso-level-number-format:bullet;
       mso-level-text:o;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Courier New";}
   @list l27:level6
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:Wingdings;}
   @list l27:level7
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:Symbol;}
   @list l27:level8
       {mso-level-number-format:bullet;
       mso-level-text:o;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:"Courier New";}
   @list l27:level9
       {mso-level-number-format:bullet;
       mso-level-text:;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;
       font-family:Wingdings;}
   @list l28
       {mso-list-id:2100714495;
       mso-list-type:hybrid;
       mso-list-template-ids:35560536 67698713 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l28:level1
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:.75in;
       text-indent:-.25in;}
   @list l28:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.25in;
       text-indent:-.25in;}
   @list l28:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.75in;
       text-indent:-9.0pt;}
   @list l28:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l28:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.75in;
       text-indent:-.25in;}
   @list l28:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:3.25in;
       text-indent:-9.0pt;}
   @list l28:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l28:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.25in;
       text-indent:-.25in;}
   @list l28:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.75in;
       text-indent:-9.0pt;}
   @list l29
       {mso-list-id:2134588709;
       mso-list-type:hybrid;
       mso-list-template-ids:-301837680 67698715 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l29:level1
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:1.25in;
       text-indent:-9.0pt;}
   @list l29:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l29:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l29:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l29:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l29:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l29:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l29:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       text-indent:-.25in;}
   @list l29:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       text-indent:-9.0pt;}
   @list l30
       {mso-list-id:2138715676;
       mso-list-type:hybrid;
       mso-list-template-ids:275535248 67698703 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
   @list l30:level1
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:1.75in;
       text-indent:-.25in;}
   @list l30:level2
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:2.25in;
       text-indent:-.25in;}
   @list l30:level3
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:2.75in;
       text-indent:-9.0pt;}
   @list l30:level4
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.25in;
       text-indent:-.25in;}
   @list l30:level5
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:3.75in;
       text-indent:-.25in;}
   @list l30:level6
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:4.25in;
       text-indent:-9.0pt;}
   @list l30:level7
       {mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:4.75in;
       text-indent:-.25in;}
   @list l30:level8
       {mso-level-number-format:alpha-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:left;
       margin-left:5.25in;
       text-indent:-.25in;}
   @list l30:level9
       {mso-level-number-format:roman-lower;
       mso-level-tab-stop:none;
       mso-level-number-position:right;
       margin-left:5.75in;
       text-indent:-9.0pt;}
   ol
       {margin-bottom:0in;}
   ul
       {margin-bottom:0in;}
   -->
   </style>

.. raw:: html

   <!--[if gte mso 10]>
   <style>
    /* Style Definitions */
    table.MsoNormalTable
       {mso-style-name:"Table Normal";
       mso-tstyle-rowband-size:0;
       mso-tstyle-colband-size:0;
       mso-style-noshow:yes;
       mso-style-priority:99;
       mso-style-parent:"";
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   table.MsoTableGrid
       {mso-style-name:"Table Grid";
       mso-tstyle-rowband-size:0;
       mso-tstyle-colband-size:0;
       mso-style-unhide:no;
       border:solid black 1.0pt;
       mso-border-alt:solid black .5pt;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-border-insideh:.5pt solid black;
       mso-border-insidev:.5pt solid black;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Times New Roman",serif;
       mso-fareast-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   table.MsoTableLightShadingAccent2
       {mso-style-name:"Light Shading - Accent 2";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:60;
       mso-style-unhide:no;
       border-top:solid #C0504D 1.0pt;
       border-left:none;
       border-bottom:solid #C0504D 1.0pt;
       border-right:none;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       color:#943634;
       mso-fareast-language:EN-US;}
   table.MsoTableLightShadingAccent2FirstRow
       {mso-style-name:"Light Shading - Accent 2";
       mso-table-condition:first-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #C0504D;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #C0504D;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent2LastRow
       {mso-style-name:"Light Shading - Accent 2";
       mso-table-condition:last-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #C0504D;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #C0504D;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent2FirstCol
       {mso-style-name:"Light Shading - Accent 2";
       mso-table-condition:first-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent2LastCol
       {mso-style-name:"Light Shading - Accent 2";
       mso-table-condition:last-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent2OddColumn
       {mso-style-name:"Light Shading - Accent 2";
       mso-table-condition:odd-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#EFD3D2;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.MsoTableLightShadingAccent2OddRow
       {mso-style-name:"Light Shading - Accent 2";
       mso-table-condition:odd-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#EFD3D2;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.MsoTableLightShadingAccent3
       {mso-style-name:"Light Shading - Accent 3";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:60;
       mso-style-unhide:no;
       border-top:solid #9BBB59 1.0pt;
       border-left:none;
       border-bottom:solid #9BBB59 1.0pt;
       border-right:none;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       color:#76923C;
       mso-fareast-language:EN-US;}
   table.MsoTableLightShadingAccent3FirstRow
       {mso-style-name:"Light Shading - Accent 3";
       mso-table-condition:first-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #9BBB59;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #9BBB59;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent3LastRow
       {mso-style-name:"Light Shading - Accent 3";
       mso-table-condition:last-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #9BBB59;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #9BBB59;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent3FirstCol
       {mso-style-name:"Light Shading - Accent 3";
       mso-table-condition:first-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent3LastCol
       {mso-style-name:"Light Shading - Accent 3";
       mso-table-condition:last-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent3OddColumn
       {mso-style-name:"Light Shading - Accent 3";
       mso-table-condition:odd-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#E6EED5;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.MsoTableLightShadingAccent3OddRow
       {mso-style-name:"Light Shading - Accent 3";
       mso-table-condition:odd-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#E6EED5;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.MsoTableLightShadingAccent5
       {mso-style-name:"Light Shading - Accent 5";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:60;
       mso-style-unhide:no;
       border-top:solid #4BACC6 1.0pt;
       border-left:none;
       border-bottom:solid #4BACC6 1.0pt;
       border-right:none;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       color:#31849B;
       mso-fareast-language:EN-US;}
   table.MsoTableLightShadingAccent5FirstRow
       {mso-style-name:"Light Shading - Accent 5";
       mso-table-condition:first-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4BACC6;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #4BACC6;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent5LastRow
       {mso-style-name:"Light Shading - Accent 5";
       mso-table-condition:last-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4BACC6;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #4BACC6;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent5FirstCol
       {mso-style-name:"Light Shading - Accent 5";
       mso-table-condition:first-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent5LastCol
       {mso-style-name:"Light Shading - Accent 5";
       mso-table-condition:last-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.MsoTableLightShadingAccent5OddColumn
       {mso-style-name:"Light Shading - Accent 5";
       mso-table-condition:odd-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#D2EAF1;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.MsoTableLightShadingAccent5OddRow
       {mso-style-name:"Light Shading - Accent 5";
       mso-table-condition:odd-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#D2EAF1;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.LightList1
       {mso-style-name:"Light List1";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:61;
       mso-style-unhide:no;
       border:solid black 1.0pt;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   table.LightList1FirstRow
       {mso-style-name:"Light List1";
       mso-table-condition:first-row;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-shading:black;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       color:white;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList1LastRow
       {mso-style-name:"Light List1";
       mso-table-condition:last-row;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-border-top:2.25pt double black;
       mso-tstyle-border-left:1.0pt solid black;
       mso-tstyle-border-bottom:1.0pt solid black;
       mso-tstyle-border-right:1.0pt solid black;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList1FirstCol
       {mso-style-name:"Light List1";
       mso-table-condition:first-column;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList1LastCol
       {mso-style-name:"Light List1";
       mso-table-condition:last-column;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList1OddColumn
       {mso-style-name:"Light List1";
       mso-table-condition:odd-column;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid black;
       mso-tstyle-border-left:1.0pt solid black;
       mso-tstyle-border-bottom:1.0pt solid black;
       mso-tstyle-border-right:1.0pt solid black;}
   table.LightList1OddRow
       {mso-style-name:"Light List1";
       mso-table-condition:odd-row;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid black;
       mso-tstyle-border-left:1.0pt solid black;
       mso-tstyle-border-bottom:1.0pt solid black;
       mso-tstyle-border-right:1.0pt solid black;}
   table.LightGrid-Accent11
       {mso-style-name:"Light Grid - Accent 11";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:62;
       mso-style-unhide:no;
       border:solid #4F81BD 1.0pt;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-border-insideh:1.0pt solid #4F81BD;
       mso-border-insidev:1.0pt solid #4F81BD;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   table.LightGrid-Accent11FirstRow
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:first-row;
       mso-style-priority:62;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:2.25pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:1.0pt solid #4F81BD;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       font-family:"Cambria",serif;
       mso-ascii-font-family:Cambria;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Cambria;
       mso-bidi-font-family:"Times New Roman";
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightGrid-Accent11LastRow
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:last-row;
       mso-style-priority:62;
       mso-style-unhide:no;
       mso-tstyle-border-top:2.25pt double #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:1.0pt solid #4F81BD;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       font-family:"Cambria",serif;
       mso-ascii-font-family:Cambria;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Cambria;
       mso-bidi-font-family:"Times New Roman";
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightGrid-Accent11FirstCol
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:first-column;
       mso-style-priority:62;
       mso-style-unhide:no;
       font-family:"Cambria",serif;
       mso-ascii-font-family:Cambria;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Cambria;
       mso-bidi-font-family:"Times New Roman";
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightGrid-Accent11LastCol
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:last-column;
       mso-style-priority:62;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;
       font-family:"Cambria",serif;
       mso-ascii-font-family:Cambria;
       mso-fareast-font-family:"Times New Roman";
       mso-hansi-font-family:Cambria;
       mso-bidi-font-family:"Times New Roman";
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightGrid-Accent11OddColumn
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:odd-column;
       mso-style-priority:62;
       mso-style-unhide:no;
       mso-tstyle-shading:#D3DFEE;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;}
   table.LightGrid-Accent11OddRow
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:odd-row;
       mso-style-priority:62;
       mso-style-unhide:no;
       mso-tstyle-shading:#D3DFEE;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;
       mso-tstyle-border-insidev:1.0pt solid #4F81BD;}
   table.LightGrid-Accent11EvenRow
       {mso-style-name:"Light Grid - Accent 11";
       mso-table-condition:even-row;
       mso-style-priority:62;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;
       mso-tstyle-border-insidev:1.0pt solid #4F81BD;}
   table.LightShading-Accent11
       {mso-style-name:"Light Shading - Accent 11";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:60;
       mso-style-unhide:no;
       border-top:solid #4F81BD 1.0pt;
       border-left:none;
       border-bottom:solid #4F81BD 1.0pt;
       border-right:none;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       color:#365F91;
       mso-fareast-language:EN-US;}
   table.LightShading-Accent11FirstRow
       {mso-style-name:"Light Shading - Accent 11";
       mso-table-condition:first-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightShading-Accent11LastRow
       {mso-style-name:"Light Shading - Accent 11";
       mso-table-condition:last-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightShading-Accent11FirstCol
       {mso-style-name:"Light Shading - Accent 11";
       mso-table-condition:first-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightShading-Accent11LastCol
       {mso-style-name:"Light Shading - Accent 11";
       mso-table-condition:last-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightShading-Accent11OddColumn
       {mso-style-name:"Light Shading - Accent 11";
       mso-table-condition:odd-column;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#D3DFEE;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.LightShading-Accent11OddRow
       {mso-style-name:"Light Shading - Accent 11";
       mso-table-condition:odd-row;
       mso-style-priority:60;
       mso-style-unhide:no;
       mso-tstyle-shading:#D3DFEE;
       mso-tstyle-border-left:cell-none;
       mso-tstyle-border-right:cell-none;
       mso-tstyle-border-insideh:cell-none;
       mso-tstyle-border-insidev:cell-none;}
   table.LightList-Accent11
       {mso-style-name:"Light List - Accent 11";
       mso-tstyle-rowband-size:1;
       mso-tstyle-colband-size:1;
       mso-style-priority:61;
       mso-style-unhide:no;
       border:solid #4F81BD 1.0pt;
       mso-padding-alt:0in 5.4pt 0in 5.4pt;
       mso-para-margin:0in;
       mso-para-margin-bottom:.0001pt;
       mso-pagination:widow-orphan;
       font-size:10.0pt;
       font-family:"Calibri",sans-serif;
       mso-bidi-font-family:"Times New Roman";
       mso-fareast-language:EN-US;}
   table.LightList-Accent11FirstRow
       {mso-style-name:"Light List - Accent 11";
       mso-table-condition:first-row;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-shading:#4F81BD;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       color:white;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList-Accent11LastRow
       {mso-style-name:"Light List - Accent 11";
       mso-table-condition:last-row;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-border-top:2.25pt double #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;
       mso-para-margin-top:0in;
       mso-para-margin-bottom:0in;
       mso-para-margin-bottom:.0001pt;
       line-height:normal;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList-Accent11FirstCol
       {mso-style-name:"Light List - Accent 11";
       mso-table-condition:first-column;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList-Accent11LastCol
       {mso-style-name:"Light List - Accent 11";
       mso-table-condition:last-column;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-ansi-font-weight:bold;
       mso-bidi-font-weight:bold;}
   table.LightList-Accent11OddColumn
       {mso-style-name:"Light List - Accent 11";
       mso-table-condition:odd-column;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;}
   table.LightList-Accent11OddRow
       {mso-style-name:"Light List - Accent 11";
       mso-table-condition:odd-row;
       mso-style-priority:61;
       mso-style-unhide:no;
       mso-tstyle-border-top:1.0pt solid #4F81BD;
       mso-tstyle-border-left:1.0pt solid #4F81BD;
       mso-tstyle-border-bottom:1.0pt solid #4F81BD;
       mso-tstyle-border-right:1.0pt solid #4F81BD;}
   </style>
   <![endif]-->

.. raw:: html

   <!--[if gte mso 9]><xml>
    <o:shapedefaults v:ext="edit" spidmax="2049"/>
   </xml><![endif]-->

.. raw:: html

   <!--[if gte mso 9]><xml>
    <o:shapelayout v:ext="edit">
     <o:idmap v:ext="edit" data="1"/>
    </o:shapelayout></xml><![endif]-->

.. raw:: html

   </head>

.. raw:: html

   <body lang="EN-US" link="blue" vlink="purple" style="tab-interval:.5in">

.. raw:: html

   <div class="WordSection1">

.. raw:: html

   <p class="MsoTitle">

 F5 Networks Agility 2018: LTM Fundamentals v13.1

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

Participant Hands-on Lab Guide

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-bottom:0in;margin-bottom:.0001pt">

.. raw:: html

   </p>

.. raw:: html

   <p class="DocumentType" style="margin-top:0in;margin-right:0in;margin-bottom:
   0in;margin-left:315.0pt;margin-bottom:.0001pt;text-indent:.5in">

Last Updated: 7/17/2018

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <div class="WordSection2">

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoFooter">

©2018 F5 Networks, Inc. All rights reserved. F5, F5 Networks, and the F5
logo are trademarks of F5 Networks, Inc. in the U.S. and in certain
other countries. Other F5 trademarks are identified at f5.com.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoFooter">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoFooter">

Any other products, services, or company names referenced herein may be
trademarks of their respective owners with no endorsement or
affiliation, express or implied, claimed by F5.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoFooter">

 

.. raw:: html

   </p>

.. raw:: html

   <h1>

 

.. raw:: html

   </h1>

.. raw:: html

   <h1>

Table of Contents

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoToc2">

.. raw:: html

   <!--[if supportFields]><u><span style='mso-bidi-font-size:
   11.0pt;font-family:"Cambria",serif;mso-ascii-theme-font:major-latin;mso-hansi-theme-font:
   major-latin;mso-bidi-font-weight:bold'><span style='mso-element:field-begin'></span><span
   style='mso-spacerun:yes'> </span>TOC \o &quot;2-3&quot; \t &quot;Heading
   1,2,Contents,1,Appendix Heading1,1,Index Title,1,SectionHeader,1&quot; <span
   style='mso-element:field-separator'></span></span></u><![endif]-->

Table of
Contents........................................................................................................................................
3

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

BIG-IP® Local Traffic Manager (LTM) - V13.1 Lab
Guide.................................................................................
7

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab
Overview..............................................................................................................................................
7

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Scenario.....................................................................................................................................................
8

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab Network Diagram (based on
Lamp3.6)...................................................................................................
8

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 1: Access the Lab
Environment..............................................................................................................
8

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Access the Lab
Environment.........................................................................................................................
9

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 2: The Basics (Networking, Pools and Virtual
Servers)...........................................................................
11

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Creating
VLANs........................................................................................................................................
11

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Assigning a Self IP addresses to your
VLANs...................................................................................................
13

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Assigning the Default
Gateway...................................................................................................................
15

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Creating
Pools.........................................................................................................................................
16

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Creating Virtual
Servers.............................................................................................................................
17

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

ExtraCredit!.............................................................................................................................................
20

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 3: Load Balancing, Monitoring and
Persistence.....................................................................................
22

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Ratio Load
Balancing................................................................................................................................
22

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Priority Groups
Lab...................................................................................................................................
24

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Monitor
Labs...........................................................................................................................................
26

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Content
Monitors.....................................................................................................................................
27

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Monitor
Testing.......................................................................................................................................
31

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Persistence
Labs.......................................................................................................................................
32

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Simple (Source Address)
Persistence.............................................................................................................
32

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Cookie Persistence (Cookie
Insert)................................................................................................................
36

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 4: Accelerating Applications
Lab..........................................................................................................
39

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

TCP
Express.............................................................................................................................................
39

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

HTTP Optimization - RamCache
Lab.............................................................................................................
40

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

HTTP Optimization - HTTP Compression
Lab..................................................................................................
42

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 5: SSL Offload and
Security..................................................................................................................
43

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Creating a Self-signed certificate and
key......................................................................................................
43

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Creating SSL Client
Profile..........................................................................................................................
45

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Building our New Secure Virtual
Server.........................................................................................................
46

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Securing Web Applications with the HTTP
profile............................................................................................
47

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 6: BIG-IP Policies and
iRules.................................................................................................................
49

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Using the Builtiin https\_redirect
iRule...........................................................................................................
49

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Use a BIG-IP Policy to retrieve images from a different
pool..............................................................................
50

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Use an iRule to Retrieve Images From a Different
Pool.....................................................................................
52

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 7: Support and
Troubleshooting..........................................................................................................
53

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Archive the current configuration and perform a health check using a
QKview..................................................... 53

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Troubleshoot using TCPDump or
Curl............................................................................................................
54

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Lab 8: Device Service Clusters
(DSC)...........................................................................................................
56

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Base Networking and HA
VLAN...................................................................................................................
56

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Configure
HA...........................................................................................................................................
57

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Bonus Lab – Traffic groups, iApps and
Active-Active....................................................................................
59

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Building a new traffic group and floating
IP...................................................................................................
59

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Building an HTTP application using an iApp
template......................................................................................
59

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

Active-Active
Setup...................................................................................................................................
60

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc2">

Appendix..................................................................................................................................................
61

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoToc3">

BIG-IP Policy for retrieving jpeg images from the
image\_pool...........................................................................
61

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

.. raw:: html

   <!--[if supportFields]><u><span style='mso-bidi-font-size:
   11.0pt;font-family:"Cambria",serif;mso-ascii-theme-font:major-latin;mso-hansi-theme-font:
   major-latin;mso-bidi-font-family:Calibri;mso-bidi-theme-font:minor-latin;
   mso-bidi-language:HE;mso-bidi-font-weight:bold;mso-no-proof:yes'><span
   style='mso-element:field-end'></span></span></u><![endif]-->

 

.. raw:: html

   </p>

.. raw:: html

   <h1>

 

.. raw:: html

   </h1>

.. raw:: html

   <h1>

BIG-IP® Local Traffic Manager (LTM) - V13.1 Lab Guide

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

This lab guide is designed for you to get an understanding of the BIG-IP
Local Traffic Manager (LTM) product.

.. raw:: html

   </p>

.. raw:: html

   <h2 style="margin-left:0in;text-indent:0in;tab-stops:.5in">

Lab Overview

.. raw:: html

   </h2>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="text-indent:-.25in;mso-list:l27 level1 lfo4">

<[if !supportLists]>·       <[endif]>F5 BIG-IP LTM VE, licensed using
F5-BIG-VE-LAB-LIC

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="text-indent:-.25in;mso-list:l27 level1 lfo4">

<[if !supportLists]>·       <[endif]>Your BIG-IP is as close to factory
default as possible. Only the following changes have been made:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.0in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l27 level2 lfo4">

<[if !supportLists]>o   <[endif]>The management IP has already been
configured

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.0in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l27 level2 lfo4">

<[if !supportLists]>o   <[endif]>The initial setup has been completed. 
(Licensing and Platform information)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.0in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l27 level2 lfo4">

<[if !supportLists]>o   <[endif]>The Idle Timeout was modified from 1200
seconds to 7200 seconds

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.0in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l27 level2 lfo4">

<[if !supportLists]>o   <[endif]>The Welcome messages for the GUI and
SSH were changed.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.0in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l27 level2 lfo4">

<[if !supportLists]>o   <[endif]>An archive file
base-setup-and-licensing.ucs was created allowing you to revert to the
base settings above.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

Various directory and application services are available within the lab
environment.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="GenericSectionHeader">

DO NOT COPY INFORMATION FROM THE SCREENSHOTS.  THEY ARE FOR REFERENCE
ONLY.

.. raw:: html

   </p>

.. raw:: html

   <h2 style="margin-left:0in;text-indent:0in;tab-stops:.5in">

 

.. raw:: html

   </h2>

.. raw:: html

   <h2 style="margin-left:0in;text-indent:0in;tab-stops:.5in">

Scenario

.. raw:: html

   </h2>

.. raw:: html

   <p class="MsoNormal">

Your customer has the following environment.  The servers sit on the
customers internal VLANs, the virtual servers will exist in another VLAN
in the DMZ.  The customer does not want to rework their networking and
does not wish to use the LTM as the default gateway.  Our solution will
be to use SNATs to force traffic to pass through the BIG-IP to return
through the LTM.

.. raw:: html

   </p>

.. raw:: html

   <h1>

Lab Network Diagram (based on Lamp3.6)

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoBodyText" style="margin-left:-31.5pt">

.. raw:: html

   </p>

.. raw:: html

   <h1>

Lab 1: Access the Lab Environment

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

You will now gain access to your lab environment and your BIG-IP.  The
first agenda item is to log in to the training portal.  After this, you
will create a remote desktop session to the training environment and
access your BIG-IP.

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Access the Lab Environment

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.25in;text-indent:-.25in;mso-list:l22 level1 lfo3">

<[if !supportLists]>1.     <[endif]>Using Firefox or Chrome open a
connection to the training portal supplied by the instructor

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.75in;text-indent:-.25in;mso-list:l22 level2 lfo3">

<[if !supportLists]>a.     <[endif]>Using the IP address supplied by the
instructor log on to the training portal

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                      i.    
<[endif]>http://<ip\_address\_supplied\_by\_instructor/

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:81.0pt">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                     ii.    
<[endif]>User:          ltm101studentX (where X is your student number)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                    iii.    
<[endif]>Password:   PieINtheSKYltm101

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.75in;text-indent:-.25in;mso-list:l22 level2 lfo3">

<[if !supportLists]>b.     <[endif]>Open the blueprint or the view link.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.5in">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.75in;text-indent:-.25in;mso-list:l22 level2 lfo3">

<[if !supportLists]>c.      <[endif]>Find the Xunbutu jumpbox in the
list of applications and select console to access the jumpbox via the
browser.  Alternately you can use the IP address associated with the
jumpbox to access it via RDP.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.5in">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.75in;text-indent:-.25in;mso-list:l22 level2 lfo3">

<[if !supportLists]>d.     <[endif]>Access the xbun-jumpbox using the
Console (watch for pop-up blockers)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                      i.    
<[endif]>User:          f5student  

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                     ii.    
<[endif]>Password:  f5DEMOs4u

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.25in;text-indent:-.25in;mso-list:l22 level1 lfo3">

<[if !supportLists]>2.     <[endif]>To access the BIG-IP open a new
browser window and

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:.75in;text-indent:-.25in;mso-list:l22 level2 lfo3">

<[if !supportLists]>a.     <[endif]>Click the bookmark bigip01

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                      i.    
<[endif]>User:  admin 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:2.0pt;margin-right:0in;margin-bottom:2.0pt;
   margin-left:1.25in;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:
   l22 level3 lfo3">

<[if !supportLists]>                                     ii.    
<[endif]>Password: admin

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo5">

<[if !supportLists]>b.     <[endif]>Nomenclature for GUI navigation
begins on the side-bar and then goes to the pop-up or
top-bar.                

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                      i.    
<[endif]> For example:  Go to Local Traffic >> Virtual Servers >>
Virtual Servers List

.. raw:: html

   </p>

.. raw:: html

   <h1>

Lab 2: The Basics (Networking, Pools and Virtual Servers)

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

In this lab we will access the Management GUI.  We will then create the
VLANs and assign self IP addresses to our VLAN.  As mentioned during our
lecture portion, BIG-IPs may be put in-line or one-armed depending on
your customer’s requirements and topology. 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Creating VLANs

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.25in">

You will need create two untagged VLANs, one client-side VLAN
(client\_vlan) and one server-side VLAN (server\_vlan) for the devices
in your network.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo22">

<[if !supportLists]>1.     <[endif]>From the sidebar select Network >>
VLANs then select Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Under General Properties:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Name:  client\_vlan

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>The name is for management purposes
only, you could name them after your children or pets

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Tag: <leave blank>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>Entering a tag is only required for
“Tagged” (802.1q) interfaces. “Untagged” interfaces will automatically
get a tag which is used for internal L2 segmentation of traffic.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>c.      <[endif]>Under Resources in the Interfaces
section:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Interface: 1.1

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Tagging: Untagged

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Select the Add button.  Leave all other items at the default
setting.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>When you have completed your VLAN configuration, hit the
Finished button

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51">

Create another untagged VLAN named server\_vlan on interface 1.2.

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Assigning a Self IP addresses to your VLANs

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo23">

<[if !supportLists]>1.     <[endif]>Go to Network >> Self IPs, select
Create.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Create a new self IP, for the
server\_vlan and client\_vlan VLANs. In Network >> Self IPs >> New Self
IP, under Configuration enter:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:2.0in;text-indent:.5in">

Server-Side                  Client-side

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Name:                    server\_ip                    
client\_ip

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>IP Address:             10.1.20.245                 10.1.10.245

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Netmask:                255.255.255.0             
255.255.255.0

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>VLAN:                     server\_vlan                 
client\_vlan

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     v.    
<[endif]>Port Lockdown:      Allow None                  Allow None

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>The default “Allow None” means the
Self IP would respond only to ICMP.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>2.     <[endif]>The “Allow Defaults” selection opens
the following on the self IP of the VLAN

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>a.     <[endif]>TCP:  ssh, domain, snmp, https

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>b.     <[endif]>TCP: 4353, 6699 (for F5 protocols,
such as HA and iQuery)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>c.      <[endif]>UDP: 520, cap, domain, f5-iquery,
snmp

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>d.     <[endif]>PROTOCOL: ospf

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>3.     <[endif]>NOTE: Even with “Allow None” chosen,
traffic destined for a virtual server or object on the F5 (e.g. NAT) are
able to pas through without issue as any object created on the F5 is by
default allowed to pass through.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>When you have completed your self-IP
configuration, hit the  button.  You should have something similar to
the following:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Assigning the Default Gateway

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo24">

<[if !supportLists]>1.     <[endif]>Go to Network > Routes and then Add.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Here is where we assign our default
gateway (and other static routes as desired)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>Under Properties

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Name:                    default\_gateway

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Destination:           0.0.0.0

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Netmask:                0.0.0.0

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>Resource:               Use Gateway…

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     v.    
<[endif]>Gateway Address:   10.1.10.1

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    vi.    
<[endif]>When you have completed defining your default gateway, hit the
 button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>2.     <[endif]>Verify your network configuration

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Ping your client-side self IP
(10.1.10.245) to verify connectivity       

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>Use an SSH utility, such as puTTY,
to access your BIG-IP management port at 10.1.1.245.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                      i.    
<[endif]>User: root   Password: default

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                     ii.    
<[endif]>Ping your default gateway, 10.1.10.1

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                    iii.    
<[endif]>Ping a web server at 10.1.20.11.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.25in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Creating Pools

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

In this lab we will build a pool and virtual server to support our web
site and verify our configurations by accessing our web servers through
the BIG-IP.  Verification will be performed visually and through various
statistical interfaces.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l20 level1 lfo57">

<[if !supportLists]>1.     <[endif]>From the sidebar, select Local
Traffic >> Pools then select Create. Here we will create our new pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo5">

<[if !supportLists]>c.      <[endif]>Under Configuration:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                      i.    
<[endif]>Name:  www\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo5">

<[if !supportLists]>1.     <[endif]>The name is for management purposes
only, no spaces can be used

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                     ii.    
<[endif]>Description: <optional>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                    iii.    
<[endif]>Health Monitor: http

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo5">

<[if !supportLists]>d.     <[endif]>Under Members:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                      i.    
<[endif]>Load Balancing Method: <leave at the default Round Robin>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                     ii.    
<[endif]>Priority Group Activation: <leave at default>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo5">

<[if !supportLists]>                                    iii.    
<[endif]>New Members:

.. raw:: html

   </p>

.. raw:: html

   <table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0" style="margin-left:1.5in;border-collapse:collapse;border:none;mso-border-alt:
    solid black .5pt;mso-yfti-tbllook:1184;mso-padding-alt:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes">

.. raw:: html

   <td valign="top" style="border:solid black 1.0pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

Address

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="top" style="border:solid black 1.0pt;border-left:none;mso-border-left-alt:
     solid black .5pt;mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

Service Port

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr style="mso-yfti-irow:1">

.. raw:: html

   <td valign="top" style="border:solid black 1.0pt;border-top:none;mso-border-top-alt:
     solid black .5pt;mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

10.1.20.11

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="top" style="border-top:none;border-left:none;border-bottom:solid black 1.0pt;
     border-right:solid black 1.0pt;mso-border-top-alt:solid black .5pt;
     mso-border-left-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

80

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr style="mso-yfti-irow:2">

.. raw:: html

   <td valign="top" style="border:solid black 1.0pt;border-top:none;mso-border-top-alt:
     solid black .5pt;mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

10.1.20.12

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="top" style="border-top:none;border-left:none;border-bottom:solid black 1.0pt;
     border-right:solid black 1.0pt;mso-border-top-alt:solid black .5pt;
     mso-border-left-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

80

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr style="mso-yfti-irow:3;mso-yfti-lastrow:yes">

.. raw:: html

   <td valign="top" style="border:solid black 1.0pt;border-top:none;mso-border-top-alt:
     solid black .5pt;mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

10.1.20.13

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td valign="top" style="border-top:none;border-left:none;border-bottom:solid black 1.0pt;
     border-right:solid black 1.0pt;mso-border-top-alt:solid black .5pt;
     mso-border-left-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

80

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo5">

<[if !supportLists]>1.     <[endif]>As you enter each IP address and
port combination, hit the Add button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo5">

<[if !supportLists]>e.     <[endif]>When you have completed your pool
configuration, hit the Finished button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" style="page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Creating Virtual Servers

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

Now let’s build our virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo8">

<[if !supportLists]>1.     <[endif]>Under Local Traffic >> Virtual
Servers, click the “+” icon

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Under General Properties

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Name: www\_vs

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Description: <optional>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>Type: Standard

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iv.    
<[endif]>Source/Address: <leave blank>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>Note: The default is 0.0.0.0/0, all
source IP address are allowed

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     v.    
<[endif]>Destination Address/Mask: 10.1.10.100

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>NOTE:  The default mask is /32

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    vi.    
<[endif]>Service Port: 80 or HTTP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Under Configurations

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>The web servers do not use the BIG-IP LTM as the default
gateway.  This means return traffic will route around the BIG-IP LTM and
the TCP handshake will fail.  To prevent this we can configure SNAT
Automap on the Virtual Server.  This will translate the client IP to the
self IP of the egress VLAN and ensure the response returns to the
BIG-IP.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Source Address Translation: Auto Map

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="margin-left:.25in;text-align:center;
   page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Under Resources

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>iRules: none

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Default Pool:  From the drop down menu, select the pool
(www\_pool) which you created earlier

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>Default Persistence Profile:   None

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iv.    
<[endif]>Fallback Persistence Profile: None

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>2.     <[endif]>When you have completed your virtual
server configuration, hit the Finished button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>3.     <[endif]>You have now created a Virtual
Server (Note: Items in blue are links)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>4.     <[endif]>Now let’s see if our virtual server
works!

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Open the browser to the Virtual
Server you just created

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Refresh the browser screen several
times (use “<ctrl>” F5)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo5">

<[if !supportLists]>c.      <[endif]>Go to your BIG-IP and view the
statistics for the www\_vs virtual server and the www\_pool pool and its
associated members

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo5">

<[if !supportLists]>d.     <[endif]>Go to Statistics > Module Statistics
> Local Traffic

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Choose Virtual Servers from drop down

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>e.     <[endif]>Go to Local Traffic >> Virtual
Servers>Statistics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>f.      <[endif]>Go to Local Traffic >> Pools >>
Statistics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Did each pool member receive the same number of connections?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Did each pool member receive approximately the same number of
bytes?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>Note the Source and Destination address when you go to directly
and through the virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo5">

<[if !supportLists]>5.     <[endif]>Let’s archive our configuration in
case we have to fall back later.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>Go to System >> Archives and select
Create.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                      i.    
<[endif]>Name your archive lab2\_the\_basics\_net\_pool\_vs

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Extra Credit!

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

You can also review statistics via the CLI!  Simply SSH in to the
management IP of your BIG-IP.  Refer to your Student Information page
and Network Diagram for the address.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo9">

<[if !supportLists]>1.     <[endif]>Check out the Linux CLI and TMSH

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo9">

<[if !supportLists]>a.     <[endif]>Username: root Password: default
(these are defaults)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Select VT100 as the terminal type

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Review the information of the following commands:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                   iii.    
<[endif]>bigtop –n

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>Type q to quit.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Take a look at the TMOS CLI, type
“tmsh” to enter the Traffic Management Shell.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>(tmos)# show ltm pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>(tmos)# show ltm pool detail

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>show statistics from all pools

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>(tmos)# show ltm virtual

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iv.    
<[endif]>(tmos)# show ltm virtual detail

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>Show statistics of all virtual
servers

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>2.     <[endif]>Build an FQDN pool.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Go to System  ››  Configuration :
Device : DNS

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>In the DNS Lookup Server List, in the Address box enter
10.1.20.252, hit the Add button.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>This is the lab DNS server. Don’t
forget to Update.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>From the Linux CLI do a dig fqdnpool.f5demo.com.  You will see
IP addresses for that name.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Go to Local Traffic  ››  Pools :
Pool List and select Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Name the pool fqdn\_pool and give the pool an http monitor.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>In New Members, select the New FQDN Node button. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>The FQDN is fqdnpool.f5demo.com and
the Server Port is 8081.  Hit Add and Finished.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>You will see the BIG-IP queried the
DNS server and built a pool based on the answered.  Modifying the FQDN
on the name server will cause the pool to be modified.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>3.     <[endif]>Check out the Dashboard!

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Go to Statistics>Dashboard

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>4.     <[endif]>Click the Big Red F5 ball.  This
will take you to the Welcome page.  Here you can find links to:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>User Documentation, Running the
Setup Utility, Support, Plug-ins, SNMP MIBs

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <h1>

Lab 3: Load Balancing, Monitoring and Persistence

.. raw:: html

   </h1>

.. raw:: html

   <p class="Objective">

Objectives:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Configure and review Ratio load
balancing

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Build and test priority groups

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Build a content monitor that looks
for a receive string and requires authentication

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Build and review simple (source IP)
persistence and cookie persistence.

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Ratio Load Balancing

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo25">

<[if !supportLists]>5.     <[endif]>Go to Local Traffic >> Pools and
select www\_pool and then Members from the top bar or you could click on
the Members link in the Pool List screen.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Note: When we created the pool, we
performed all of our configurations on one page, but when we modify a
pool the Resource information is under the Members tab

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>6.     <[endif]>Under Load Balancing section

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Change the Load Balancing Method to
Ratio (Member)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>As you look at the drop-down menu,
notice most load balancing methods have two options: (Node) or (Member).
Remember the difference?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Don’t forget the Update button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>d.     <[endif]>Then under Current Members

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Select the first member in the pool 10.1.20.11:80.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Under the Configuration section

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>Change the Ratio of the member to 3

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo25">

<[if !supportLists]>e.     <[endif]>Select the Update button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level1 lfo25">

<[if !supportLists]>7.     <[endif]>Verification

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Check the pool statistics by
selecting Statistics on the top bar, if you are still in Local Traffic
>> Pools, or by going to Statistics >> Module Statistics >> Local
Traffic and selecting Pool from Statistics Type.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Reset the statistics for your
www\_pool pool by checking the boxes next to the pool members and
hitting the Reset button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Browse to your www\_vs (10.1.10.100) virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Refresh the browser screen several times (use “<ctrl>” F5)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>Select the Refresh button on the Statistics screen

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iv.    
<[endif]>How many total connections has each member taken?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     v.    
<[endif]>Is the ratio of connections correct between the members?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Now go back and put the pool load
balancing method back to Round Robin

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Reset the statistics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Refresh the virtual server page several times

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>Refresh the statistics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iv.    
<[endif]>Does the ratio setting have any impact now?

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Priority Groups Lab

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

Let’s look at priority groups.  In this scenario we will treat the .13
server as if it were in a disaster recovery site that can be reached
over a backhaul.  The customer would like to maintain at least two
members in the pool for redundancy and load.  They would find this
beneficial to allow connections to proceed during a maintenance window
or during an outage.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo10">

<[if !supportLists]>1.     <[endif]>Go to Local Traffic >> Pools >>
www\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Select the Members tab.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Set the Load Balancing Method back to Round Robin

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Set the Priority Group Activation to Less than … 2 Available
Members.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Don’t forget to hit the Update
button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Select the pool members
10.128.20.11 and 10.128.20.12 and set their Priority Group to 2.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>This will allow you to change the priority on that particular
member.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>2.     <[endif]>Review your settings and let’s see
how load balancing reacts now

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Select the Statistics tab.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Reset the pool statistics.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Browse to your virtual server and
refresh several times.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>d.     <[endif]>Refresh your statistics.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>e.     <[endif]>Are all members taking connections?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>f.      <[endif]>Which member isn’t taking
connections?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>3.     <[endif]>Let’s simulate a maintenance window
or an outage by disabling a pool member in the highest priority group
(2). 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

NOTE: F5 ranks priority from low number to high number.  This means, a
priority of 1 has a lower priority than 2, and onwards.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.25in;mso-add-space:auto">

This should cause priority group activation to kick in, since the number
of active members in our high priority group has dropped below one.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>4.     <[endif]>Select the member in the Priority
Group 2 and Disable that pool member.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Select the Disable button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center;
   page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>The status indicator now goes to
black, indicating the member has been disabled

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>5.     <[endif]>Once again, select Statistics, reset
the pool statistics, browse to the virtual server and see which pool
members are taking hits now.

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;tab-stops:321.0pt;background:#FDE9D9;mso-background-themecolor:
   accent6;mso-background-themetint:51">

Once you are done testing re-enable your disabled pool member.        

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Monitor Labs

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="Objective">

Objective:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Build a default monitor for nodes

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Build a content monitor for your
pool

.. raw:: html

   </p>

.. raw:: html

   <p class="LabReq">

Default Monitors

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo26">

<[if !supportLists]>1.     <[endif]>Go to Local Traffic >> Nodes, note
the status of the nodes.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Note that the nodes exist in this
table, even though they were never specifically configured in the Node
section of the GUI.  Each time a unique IP address is placed in a pool a
corresponding node entry is added and assigned the default monitor (if
any).

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Select the Default Monitors tab.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-top:0in;margin-right:0in;
   margin-bottom:0in;margin-left:.75in;margin-bottom:.0001pt;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Notice we have several options. For
nodes you will want a generic monitor, so we will choose icmp.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-top:0in;margin-right:0in;
   margin-bottom:0in;margin-left:.75in;margin-bottom:.0001pt;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>d.     <[endif]>Select icmp from the Available box
and hit  to place it in the Active box.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>e.     <[endif]>Click on the Update button to
finalize your changes.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>2.     <[endif]>Select Node List or Statistics from
the top tab.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>What are your node statuses?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>3.     <[endif]>Select Statistics >> Module
Statistics >> Local Traffic

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>What are the statuses of your nodes,
pool and virtual server?

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:0in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:0in;text-indent:0in;tab-stops:321.0pt;background:#FDE9D9;
   mso-background-themecolor:accent6;mso-background-themetint:51">

For those of you who did the FQDN Pool extra credit lab, you will notice
your FQDN in the node list.  The status should be Available (Green) even
though there wasn’t a monitor.  This is because a good status indicates
the BIG-IP successfully queried the DNS server for the name.  Click on
the FQDN node to see additional options, such as query
interval.                   

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Content Monitors

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

The default monitor simply tells us the IP address is accessible, but we
really don’t know the status of the particular application the node
supports.  We are now going to create a monitor to specifically test the
application we are interested in.  We are going to check our web site
and its basic authentication capabilities.  

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo28">

<[if !supportLists]>4.     <[endif]>Browse to http://10.1.10.100 and on
the web page select the Basic Authentication link under Authentication
Examples. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo28">

<[if !supportLists]>a.     <[endif]>User:          user.1

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo28">

<[if !supportLists]>b.     <[endif]>Password:   password

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo28">

<[if !supportLists]>c.      <[endif]>You could use text from this page
or text within the source code to test for availability.  You could also
use HTTP statuses or header information.  You will be looking for the
HTTP status “200 OK” as your receive string to determine availability.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo28">

<[if !supportLists]>d.     <[endif]>Note the URI is /basic.  You will
need this for your monitor.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo28">

<[if !supportLists]>5.     <[endif]>Select Local Traffic >> Monitor on
the side-bar and select the plus (+) sign or Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Now we can create a monitor to check
the content of our web page to ensure things are running properly.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Name: www\_test

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>Type: HTTP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Once you have selected you parent
(Type) monitor, you can access the Configuration section

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Send String: Enter the command to retrieve the page you want
“GET /basic/:raw-latex:`\r`:raw-latex:`\n`” (no quotes)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                     ii.    
<[endif]>In the Receive String box put “200 OK” (no quotes)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo7">

<[if !supportLists]>1.     <[endif]>NOTE: The receive string is not case
sensitive.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                    iii.    
<[endif]>Enter user.1/password for the Username and Password

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Click Finish and you will be taken
back to Local Traffic >> Monitors

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.25in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>6.     <[endif]>Where is your new Monitor?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]> Hint: Check the lower right hand
corner of the Monitors list.  Here you can go to the next page or view
all Monitors

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>You can change the number of records
displayed per page in System >> Preferences

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>7.     <[endif]>Go to Local Traffic >> Pools >>
www\_pool and choose Properties from the top bar

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Remove the http monitor from the
Active box.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Select the www\_test monitor from
the Available monitor’s window in the Configuration section and move it
to the Active window.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>8.     <[endif]>Once you have selected your parent
(Type) monitor, you can access the Configuration section

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Select Statistics from the tabs.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>What is the status of the pool and
its members?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>9.     <[endif]>Go to Local Traffic >> Virtual
Servers. What is the status of your virtual server?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Browse to your www\_vs virtual
server.  Which members are taking traffic?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Just for fun reverse the monitor. 
Now when 200 OK is returned it indicates the server is not responding
successfully.   You can see where this would be useful if you were
looking for a 404 (bad page) response.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Monitor Testing

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

There is now the ability to test monitors.  This is tremendously helpful
as you no longer need to create monitors and add them to false objects
on the BIG-IP.  The functionality is now built in to the monitor itself
to be less invasive on your infrastructure, and less time consuming all
together.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>10.  <[endif]>Go to Local Traffic >> Pools >>
www\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Under Configuration, move the active
monitor to Available

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level1 lfo7">

<[if !supportLists]>11.  <[endif]>Go to Monitors and click on http

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>a.     <[endif]>Click the Test tab

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>b.     <[endif]>Under Address plug in 10.1.20.11 and
in the port field plug in 80

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>c.      <[endif]>Click Test

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo7">

<[if !supportLists]>d.     <[endif]>Go back to Local Traffic >> Pools >>
www\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo7">

<[if !supportLists]>                                      i.    
<[endif]>Once here, move http back to Active

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Persistence Labs

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

In this lab we will configure a couple types of persistence and view
their behavior.  For persistence, profiles will have to be created and
attached to our virtual server.

.. raw:: html

   </p>

.. raw:: html

   <p class="LabReq">

Lab Requirements:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Prior to beginning the lab verify
your www\_pool has been set to the following parameters:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="margin-left:1.25in;mso-list:l4 level2 lfo34">

<[if !supportLists]>o   <[endif]>Load Balancing Method: Round Robin

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="margin-left:1.25in;mso-list:l4 level2 lfo34">

<[if !supportLists]>o   <[endif]>Priority Group Activation: Disable

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="margin-left:1.75in;mso-list:l4 level3 lfo34">

<[if !supportLists]>§  <[endif]>The members Ratio and Priority Group
mean nothing since we aren’t using Ratio load balancing and Priority
Groups are disabled.

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="margin-left:1.25in;mso-list:l4 level2 lfo34">

<[if !supportLists]>o   <[endif]>Hit Update

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="margin-left:1.25in;mso-list:l4 level2 lfo34">

<[if !supportLists]>o   <[endif]>Hit your virtual server several times,
you should see all 3 servers respond.

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Simple (Source Address) Persistence

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level1 lfo36">

<[if !supportLists]>1.     <[endif]>Go to Local Traffic >> Profiles and
select the Persistence tab.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>a.     <[endif]>From the Persistence Profiles screen
select the Create button.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>b.     <[endif]>At the New Persistence Profile
screen enter:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>Name: my-src-persist

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                     ii.    
<[endif]>Persistence Type: Source Address Affinity

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>c.      <[endif]>This will add the Configuration
section to the General Properties section.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>Note the parent profile.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>d.     <[endif]>In the Configuration section, set
the

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>Timeout: 60 seconds

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                     ii.    
<[endif]>Prefix Length: None

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level4 lfo36">

<[if !supportLists]>1.     <[endif]>This is the default and is a /32
prefix (255.255.255.255 mask).

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level4 lfo36">

<[if !supportLists]>2.     <[endif]>Each new IP address will create a
new persistence record.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                    iii.    
<[endif]>Hint: You can’t change these settings until you have checked
the Custom box.  This prevents unwanted or unauthorized changes from
within the GUI, without explicitly allowing it.  Also, it allows you to
know what has changed from the default settings.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>e.     <[endif]>You have just created your first
custom Profile.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>Note the check box for your new custom profile isn’t grayed out
and can be selected to allow you to delete the profile if desired.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level1 lfo36">

<[if !supportLists]>2.     <[endif]>Now let’s attach our new profile to
the virtual server.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>a.     <[endif]>Go to Local Traffic >> Virtual
Server and ….

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>Select www\_vs and the Resources tab or ….

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                     ii.    
<[endif]>Take the shortcut directly to the Resources of the virtual
server.  (Can you find it?)

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51">

Note: When we created the Virtual Server, everything was on a single
page. We find when we return to modify the Virtual Server the Properties
and Resources are on different pages.

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>b.     <[endif]>Set the Default Persistence Profile
to my-src-persist.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>c.      <[endif]>Don’t forget to Update before
leaving the page. (Be careful, the reminders will stop!)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>d.     <[endif]>Testing Source Address Affinity

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>At this point you may want to open a second browser window to
the management GUI.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                     ii.    
<[endif]>From one management window go to Statistics >> Module Statistic
>> Local Traffic

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                    iii.    
<[endif]>Select Persistence Records for the Statistics Type menu

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level1 lfo36">

<[if !supportLists]>3.     <[endif]>At this point you will see that the
Persistence Records statistics display has been disabled (way back in
v12.1).  A TMSH database command is required to activate it.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>a.     <[endif]>SSH to you BIG-IP at 10.1.1.245. 
Username: root Password: default

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>b.     <[endif]>At the prompt enter:  tmsh

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>c.      <[endif]>At the TMSH prompt enter the
command in the Persistence Value GUI.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>modify sys db
ui.statistics.modulestatistics.localtraffic.persistencerecords value
true

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level4 lfo36">

<[if !supportLists]>1.     <[endif]>Tab completion will make this a
little easier

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level1 lfo36">

<[if !supportLists]>4.     <[endif]>Now, in this window you can watch
your persistence records.  You may want to set Auto Refresh to 20
seconds.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level1 lfo36">

<[if !supportLists]>5.     <[endif]>In your other management GUI window
go to www\_pool and clear the member statistics.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>a.     <[endif]>Open a browser session to your
virtual server and refresh several times.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>b.     <[endif]>How many members are taking traffic?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>c.      <[endif]>Check you Persists Records window.
Are there any persistence records?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>If you are not Auto Refreshing, don’t forget to hit Refresh

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>d.     <[endif]>Refresh you web page prior to the
Age column reaching 60.  What happens?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Cookie Persistence (Cookie Insert)

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l2 level1 lfo59">

<[if !supportLists]>1.     <[endif]>Go to Local Traffic >> Profiles >>
Persistence tab and hit Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l12 level1 lfo37">

<[if !supportLists]>a.     <[endif]>Let’s name our profile
my\_cookie\_insert (original isn’t it)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l12 level1 lfo37">

<[if !supportLists]>b.     <[endif]>Our Persistence Type will be Cookie

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l12 level1 lfo37">

<[if !supportLists]>c.      <[endif]>This brings us to the Configuration
section.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l2 level1 lfo59">

<[if !supportLists]>2.     <[endif]>As you can see, the default Cookie
Method is HTTP Cookie Insert, so we won’t have to modify the Cookie
Method

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level1 lfo38">

<[if !supportLists]>a.     <[endif]>The BIG-IP will also create a cookie
name for you using a combination of “BIGipServer” and the pool name the
virtual server service.  We will take this default also.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level1 lfo38">

<[if !supportLists]>b.     <[endif]>We will use a session cookie.  Which
means the cookie is deleted when the browser is closed.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level1 lfo38">

<[if !supportLists]>c.      <[endif]>Select Finished

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level1 lfo38">

<[if !supportLists]>d.     <[endif]>Now attach your cookie persistence
profile to your virtual server’s Default Persistence Profile by:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level2 lfo38">

<[if !supportLists]>a.     <[endif]>Go to Local Traffic >> Virtual
Server >> www\_vs >> Resources tab

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level2 lfo38">

<[if !supportLists]>b.     <[endif]>Set the Default Persistence Profile
to my\_cookie\_insert

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l6 level2 lfo38">

<[if !supportLists]>c.      <[endif]>Hit Update

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l6 level1 lfo38">

<[if !supportLists]>e.     <[endif]>Whoa! Did you just get this error
message?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l6 level1 lfo38">

<[if !supportLists]>f.      <[endif]>Remember what we said earlier about
some Profiles requiring prerequisite Profiles?  Since we are looking in
the HTTP header for the cookie the prerequisite for the Cookie Profile
is the HTTP profile. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l2 level1 lfo59">

<[if !supportLists]>3.     <[endif]>We will have to go to the virtual
server to add the HTTP profile, prior to adding the Cookie Persistence
profile.  

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>a.     <[endif]>Select the Properties tab on your
virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>b.     <[endif]>Go to HTTP Profile in the
Configuration section and select the default HTTP (http) profile.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>c.      <[endif]>Hit the Update button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>d.     <[endif]>Now we can go back to the Resource
tab and add our cookie persistence profile.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level1 lfo59">

<[if !supportLists]>4.     <[endif]>Testing cookie persistence.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>a.     <[endif]>If you wish you can watch the member
statistics to validate your persistence.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>b.     <[endif]>Open a new browser session to your
virtual server and refresh several times.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>c.      <[endif]>Does the page ever change?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>d.     <[endif]>Did you hit a different server?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>e.     <[endif]>Refresh several times.  Are you
hitting the same server?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>On the web page under HTTP Request and Response Information
click the Display Cookie link.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="margin-left:0in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51">

Archive your work in the file: lab3\_lb\_monitor\_and\_persist

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <h1>

Lab 4: Accelerating Applications Lab

.. raw:: html

   </h1>

.. raw:: html

   <p class="Objective">

Objectives:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Assign client-side and server-side
profiles

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Set up caching for your web site

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Set up compression for your web
site

.. raw:: html

   </p>

.. raw:: html

   <p class="LabReq">

Lab Prerequisites:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Prior to starting this lab remove
the cookie persistence profile from your virtual server.

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

TCP Express

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo29">

<[if !supportLists]>1.     <[endif]>Set client-side and server-side TCP
profiles on your virtual server properties.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l2 level2 lfo59">

<[if !supportLists]>f.      <[endif]>In some earlier version you would
be required to select the Advanced menu to see the Client and Server
protocol profiles.  

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>e.     <[endif]>If you chose to use the Advanced
menu you would see a whole array of new options.  There are Basic and
Advanced drop downs on many of the GUI menus.  You can always see
Advanced menus by changing the preferences in System >> Preferences.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l5 level2 lfo36">

<[if !supportLists]>f.      <[endif]>From the drop-down menus place the
tcp-wan-optimized profile on the client-side and the tcp-lan-optimized
profile on the server-side.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="margin-left:.5in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

HTTP Optimization - RamCache Lab

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l10 level1 lfo39">

<[if !supportLists]>1.     <[endif]>Visit your virtual server’s web page
and refresh it several times.  Note the Source Node for the pictures of
the BIG-IPs.  They change depending on where the connection is coming
from.  The Source Node information is part of the picture.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l10 level1 lfo39">

<[if !supportLists]>2.     <[endif]>Go to Local Traffic >> Profiles >>
Services >> Web Acceleration or Acceleration >> Profiles >> Web
Acceleration

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l28 level1 lfo40">

<[if !supportLists]>a.     <[endif]>Create a new profile named
www-opt-caching using optimized-caching as the Parent Profile. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l28 level1 lfo40">

<[if !supportLists]>b.     <[endif]>Take all the defaults, no other
changes are required.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l10 level1 lfo39">

<[if !supportLists]>3.     <[endif]>Open up your www\_vs virtual server.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l16 level1 lfo41">

<[if !supportLists]>a.     <[endif]>At the HTTP Profile drop down menu
make sure http is selected.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l16 level1 lfo41">

<[if !supportLists]>b.     <[endif]>Under Acceleration at Web
Acceleration Profile select your new caching profile; www-opt-caching

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l16 level1 lfo41">

<[if !supportLists]>c.      <[endif]>Clear the statistics on your pool
and the refresh the main web page several times.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                      i.    
<[endif]>The pictures do not change.  Why do you think that is?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                     ii.    
<[endif]>Go to your pool.  Are all pool members taking connections?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l10 level1 lfo39">

<[if !supportLists]>4.     <[endif]>Now go to Statistics >> Module
Statistics >> Local Traffic on the sidebar. From the Statistics Type
drop-down menu select Profiles Summary

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l10 level1 lfo39">

<[if !supportLists]>5.     <[endif]>Select the View link next to the Web
Acceleration profile type

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l10 level1 lfo39">

<[if !supportLists]>6.     <[endif]>You can get more detailed
information on RamCache entries at the CLI level

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l3 level1 lfo42">

<[if !supportLists]>a.     <[endif]>Log onto the CLI of your BIG-IP via
SSH using the root account (user: root  password: default).

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l3 level1 lfo42">

<[if !supportLists]>b.     <[endif]>At the CLI go into tmsh at the
(tmos)# prompt

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l3 level1 lfo42">

<[if !supportLists]>c.      <[endif]>At the shell prompt enter show ltm
profile ramcache www-opt-caching

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

HTTP Optimization - HTTP Compression Lab

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo12">

<[if !supportLists]>1.     <[endif]>Go to Local Traffic >> Profiles >>
Service>HTTP Compression or Acceleration >> Profiles >> Web Acceleration

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo12">

<[if !supportLists]>a.     <[endif]>Create a new profile, www-compress,
using the wan-optimized-compression default profile.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo12">

<[if !supportLists]>2.     <[endif]>Open up your www\_vs virtual server.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l25 level1 lfo43">

<[if !supportLists]>a.     <[endif]>At the HTTP Profile drop down menu
make sure http is selected

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l25 level1 lfo43">

<[if !supportLists]>b.     <[endif]>At the Web Acceleration drop-down
menu select None

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l5 level3 lfo36">

<[if !supportLists]>                                    iii.    
<[endif]>For the purpose of this lab we don’t want caching interfering
with our response headers

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l25 level1 lfo43">

<[if !supportLists]>c.      <[endif]>At the HTTP Compression drop-down
menu select the HTTP compression profile you just created

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.25in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l20 level1 lfo57">

<[if !supportLists]>2.     <[endif]>Now open your virtual server’s web
page and under Content Examples on This Host select the HTTP Compress
Example and Plaintext Compress Example link

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l20 level2 lfo57">

<[if !supportLists]>a.     <[endif]>Now off to the statistics on the
sidebar. Under the Local Traffic drop-down menu select Profiles Summary

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l20 level2 lfo57">

<[if !supportLists]>b.     <[endif]>Select the View link next to the
HTTP Compression profile type 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" style="page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l20 level2 lfo57">

<[if !supportLists]>c.      <[endif]>On the web page under HTTP Request
and Response Information select the Request and Response Headers link.  

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l20 level3 lfo57">

<[if !supportLists]>                                      i.    
<[endif]>Notice you no longer see the Accept-Encoding header in the
Request Headers Received at the Server section

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 0in 4.0pt;background:
   #FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:51;
   margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51;border:none;mso-border-alt:solid windowtext .5pt;
   padding:0in;mso-padding-alt:1.0pt 4.0pt 0in 4.0pt">

Archive your work in a file called: lb4\_acceleration

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <h1>

Lab 5: SSL Offload and Security

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

In this Lab we will configure client-side SSL processing on the BIG-IP

.. raw:: html

   </p>

.. raw:: html

   <p class="Objective">

Objective:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Create a self-signed certificate

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Create a client SSL profile

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Modify your HTTP virtual server to
use HTTPS

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Add additional security to your
HTTPS web server using the HTTP profile

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

We will create a self-signed certificate and key for a client SSL
profile to attach to our virtual server

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Creating a Self-signed certificate and key

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo14">

<[if !supportLists]>1.     <[endif]>Go to System >> Certificate
Management >> Traffic Certificate Management >> SSL Certificate List and
select Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo14">

<[if !supportLists]>a.     <[endif]>NOTE: The default key size is 2048.
You can save SSL resources on the server-side by lowering this key size

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center;page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo13">

<[if !supportLists]>b.     <[endif]>Enter:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo13">

<[if !supportLists]>                                      i.    
<[endif]>Name: my-selfsigned-cert

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo13">

<[if !supportLists]>                                     ii.    
<[endif]>Issuer: Self

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo13">

<[if !supportLists]>                                    iii.    
<[endif]>Common Name: www.f5demo.com

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo13">

<[if !supportLists]>                                    iv.    
<[endif]>Fill out the rest any way you would like

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Creating SSL Client Profile

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo15">

<[if !supportLists]>2.     <[endif]>Go to Local Traffic >> Profiles >>
SSL >> Client menu and select Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>Under General Properties

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                      i.    
<[endif]>Name: my\_clientssl\_profile

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>b.     <[endif]>Under Configuration in the
Certificate Key Chain section, select the Custom box and hit Add

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                      i.    
<[endif]>In the Add SSL Certificate to Key Chain pop-up select:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo15">

<[if !supportLists]>1.     <[endif]>Certificate:        
my-selfsigned-cert

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo15">

<[if !supportLists]>2.     <[endif]>Key:
                    my-selfsigned-cert

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                     ii.    
<[endif]>Select Add

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>c.      <[endif]>Hit Finished.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" style="margin-left:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Building our New Secure Virtual Server

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo16">

<[if !supportLists]>1.     <[endif]>Go to Local Traffic >> Virtual
Servers and hit the Create button or hit the “+” next to Virtual Servers

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>Name:                               
            secure\_vs

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>b.     <[endif]>Destination Address/Mask:
            10.1.10.105

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>c.      <[endif]>Port:
                                              443 or HTTPS

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>d.     <[endif]>SSL Profile (Client):            
            my\_clientssl\_profile     (the profile you just created)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>e.     <[endif]>Source Address Translation:
           Auto Map                     (remember why we need this?)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>f.      <[endif]>Default Pool:                     
            www\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>g.     <[endif]>Default all other settings.  (Notice
you did not require an HTTP profile)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>h.     <[endif]>Finish

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo15">

<[if !supportLists]>2.     <[endif]>Test our secure server.  Go to you
secure\_vs at https://10.1.10.105

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>If you want to watch member traffic,
go to the www\_pool and reset the statistics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>b.     <[endif]>Browse to your secure virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>c.      <[endif]>What port did your pool members see
traffic on?

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Securing Web Applications with the HTTP profile

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo18">

<[if !supportLists]>1.     <[endif]>Let’s begin by creating a custom
HTTP profile

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>Go to Local Traffic >> Profiles >>
Services, select HTTP and create a new profile

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>b.     <[endif]>Under General Properties

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                      i.    
<[endif]>Name:                                secure-my-website

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>c.      <[endif]>Under Settings:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                      i.    
<[endif]>Set the Fallback Host:                     
http://10.1.1.252        (this will take you an internal site)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                     ii.    
<[endif]>Fallback on Error Codes:                  404                  
           (fallback site if a 404 error is received)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                    iii.    
<[endif]>Response Headers Allowed:           Content-Type Set-Cookie
Location

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo15">

<[if !supportLists]>                                    iv.    
<[endif]>Insert XForwarded For:                  
Enabled                                   (because we talked about it
earlier)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption" align="center" style="text-align:center;page-break-after:
   avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>d.     <[endif]>Attach your new HTTP Profile to your
secure (HTTPS) virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo15">

<[if !supportLists]>2.     <[endif]>Browse to your secure virtual
server.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Do web pages appear normal?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>Now browse to a bad page

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>For example, https://10.1.10.105 /badpage

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>What is the result?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>c.      <[endif]>Go to the Request and Response
Headers page. You should see a sanitized server response at the bottom
of the web page and the original client IP address

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>d.     <[endif]>You can compare the headers by
accessing your HTTP virtual server at http://10.1.10.100

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>e.     <[endif]>While you are looking at the
headers, check for the X-Forwarded-For header received by the server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast">

NOTE: Even though the data is encrypted between your browser and the
virtual server, the LTM can still modify the data (i.e. resource
cloaking) because the data is unencrypted and decompressed within TMOS

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51">

Archive your work in a file called:  lab5\_security

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <h1>

Lab 6: BIG-IP Policies and iRules

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

When clients attempt to access your secure\_vs, you don’t want them to
have to remember to type HTTPS before the web site, but you also don’t
want to open port 80 (HTTP) on your web servers as that is just asking
for trouble.  To avoid this issue, you will be creating an HTTP virtual
server that will redirect HTTP to HTTPS and the secure\_vs.   Also, you
will write an iRule and a BIG-IP policy that will retrieve images from a
different pool of servers than the default pool attached to the virtual
server.  This will give you a simple comparison between the two
methods.  You will use a policy on the HTTP server and an iRule on the
HTTPS virtual server.

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Using the Built-in https\_redirect iRule

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo19">

<[if !supportLists]>1.     <[endif]>While it would be easy to write your
own redirect iRule, note that F5 has one prebuilt that you can use

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo19">

<[if !supportLists]>a.     <[endif]>Example of simple redirect iRule:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

when HTTP\_REQUEST {

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

       HTTP::redirect https://[HTTP::host][HTTP::uri]

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

    }

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo19">

<[if !supportLists]>2.     <[endif]>Go to Local Traffic >> iRules

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo19">

<[if !supportLists]>a.     <[endif]>In the search box at the top of the
list of iRules, type redirect and hit Search.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoCaption">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo19">

<[if !supportLists]>b.     <[endif]>Open the iRule and take a quick
look.  This is an F5 Verified and supported iRule.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level1 lfo19">

<[if !supportLists]>3.     <[endif]>Create your HTTP-to-HTTPS redirect
virtual server.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>Go to Local Traffic >> Virtual
Servers and create a new virtual server.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                      i.    
<[endif]>Name:                                           
redirect\_to\_secure\_vs

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                     ii.    
<[endif]>Destination:                                   <same IP as
secure\_vs>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                    iii.    
<[endif]>Service Port:                                 80 (HTTP)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                    iv.    
<[endif]>Source Address Translation:            None <you don’t need
this as this traffic is going nowhere>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                     v.    
<[endif]>iRule:                                            
\_sys\_https\_redirect

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                    vi.    
<[endif]>Hit Finished

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo15">

<[if !supportLists]>1.     <[endif]>WOW! That didn’t go too far did it. 
You just got an error. If you are going to redirect the HTTP request,
you need the HOST and URI information and that requires the HTTP
protocol

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>b.     <[endif]>In the Configuration section make
sure the default http profile is added to the virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>c.      <[endif]>HTTP Profile: http

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>d.     <[endif]>Select Finished

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo27">

<[if !supportLists]>4.     <[endif]>Test your policy by going to
http://<ip address of your virtual>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>You should be redirected to the
HTTPS virtual server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>b.     <[endif]>As you can see, very small iRules
can make a very big difference

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Use a BIG-IP Policy to retrieve images from a different pool

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo31">

<[if !supportLists]>1.     <[endif]>Create a new pool named image\_pool,
use the http monitor for status, and add one member 10.1.20.14:80

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>2.     <[endif]>First you will create your policy
container and set your match strategy

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Try to do this using the
instructions, but a screen shot of the policy is available in the
Appendix at the end of the lab guide if you would like it

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>3.     <[endif]>Go to Local Traffic >> Policies :
Policy List and select Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Policy\_Name: access\_image\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>Strategy: Execute first matching
rule

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>c.     <[endif]>Create Policy

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="margin-left:.75in;text-align:center;
   page-break-after:avoid">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>4.     <[endif]>Now you can create/view policy rules
by selecting Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Name: get\_jpegs

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>In the box under Match all of the
following conditions: select the  to the right of All Traffic

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Use the drop-down menus to look at the HTTP URI and check if it
ends\_with an image type

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Look for JPEGs by adding jpg in the box under the any of box
and selecting Add

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>c.      <[endif]>Under Do the following when the
traffic is matched, build the following operation.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Forward Traffic to the pool named image\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>d.     <[endif]>Save

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="margin-left:.5in;text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo15">

<[if !supportLists]>5.     <[endif]>The policy is saved in Draft form
and is not available until Published.  To publish the policy:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>Select the Save Draft Policy
drop-down menu and select Save and Publish Policy

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level1 lfo15">

<[if !supportLists]>6.     <[endif]>Go to the Resources section of your
www\_vs virtual server and select Managed over the Policies box

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>Move access\_image\_pool for the
Available box to the Enabled box

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo15">

<[if !supportLists]>7.     <[endif]>Now test your change by browsing to
http://10.1.10.100

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>a.     <[endif]>If your policy is working correctly,
all of the images under F5 Platform List should be from NODE #4

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo15">

<[if !supportLists]>b.     <[endif]>Other images are PNG images and have
a different extension

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" align="center" style="text-align:center">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Use an iRule to Retrieve Images From a Different Pool

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l21 level1 lfo58">

<[if !supportLists]>1.     <[endif]>Now you will use an iRule to perform
the same image retrieval.  Your image\_pool is already created

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level1 lfo58">

<[if !supportLists]>2.     <[endif]>Go to Local Traffic >> iRules and
select Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>a.     <[endif]>Name: access\_image\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>b.     <[endif]>In the Definition section enter the
following:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>c.      <[endif]>This activity is not meant to be
“cut and paste”.  We want you to get comfortable and familiar with
typing iRules inside the GUI.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l21 level3 lfo58">

<[if !supportLists]>                                      i.    
<[endif]>Try hovering the cursor over a command or event, such as,
HTTP\_REQUEST or HTTP:uri.  You will see a definition of the item. For
example:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.25in">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l21 level1 lfo58">

<[if !supportLists]>3.     <[endif]>Save your iRule and go to the
Resources section of your secure\_vs and select iRules >> Manage

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>a.     <[endif]>Move your access\_image\_pool iRule
into the Enabled box

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l21 level1 lfo58">

<[if !supportLists]>4.     <[endif]>Test your secure\_vs virtual by
going to https://10.1.10.105

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>a.     <[endif]>The results should be the same as
before

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level1 lfo58">

<[if !supportLists]>5.     <[endif]>Extra Credit! Change both the policy
and iRule to access the image\_pool for png file types

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>a.     <[endif]>You should notice one is easier to
update than the other

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <h1>

Lab 7: Support and Troubleshooting

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

In this lab, you will review your BIG-IP using iHealth and perform some
basic troubleshooting commands

.. raw:: html

   </p>

.. raw:: html

   <p class="Objective">

Objective:

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Collect a QKView and upload it to
http://ihealth.f5.com and review the results

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Perform a TCPDump to watch traffic
flow

.. raw:: html

   </p>

.. raw:: html

   <p class="BulletedPoints" style="mso-list:l4 level1 lfo34">

<[if !supportLists]>·       <[endif]>Obtain web page information via
Curl

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Archive the current configuration and perform a health check using a
QKview

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo30">

<[if !supportLists]>1.     <[endif]>Obtain a QKView.  Go to System >>
Support

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>b.     <[endif]>Click New Support Snapshot

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

NOTE: If you have an iHealth account, you can choose to use the Generate
and Upload QKview to iHealth option as long as your management port has
Internet access.  For this exercise, we will skip this.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l21 level2 lfo58">

<[if !supportLists]>c.      <[endif]>From the drop-down, select Generate
QKview

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>Select Download and download the
QKView to your PC

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>b.     <[endif]>NOTE: If you leave the Support page
and return you will still the Support Snapshot screen.  You CANNOT
create another QKView or TCP Dump until the QKView is deleted.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo27">

<[if !supportLists]>2.     <[endif]>Import the QKView into iHealth.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>Go to http://ihealth.f5.com. If you
don’t have an account, now is the time to create one and then skip to
the next section “Troubleshoot using TCPDump or Curl” because it will
take time for your account set up.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>b.     <[endif]>Select the Upload button and upload
the QKView file you download from your BIG-IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>c.      <[endif]>Once the file is uploaded, you can
click on the hostname to view you the heuristics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                      i.    
<[endif]>Note the Diagnostics.  Go to Diagnostics >> Critical on the
side-bar. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo27">

<[if !supportLists]>1.     <[endif]>Example: The configuration contains
user accounts with insecure passwords is because we are using default
passwords

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                     ii.    
<[endif]>Select Network >> Virtual Servers, then click on the small
white triangles to expand the view or go to Pools, then Pool Members to
continue to expand the view.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo27">

<[if !supportLists]>1.     <[endif]>This is a little more detailed than
Local Traffic >> Network Map

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>d.     <[endif]>If you want to see some interesting
CLI commands, go to Commands >> Standard and expand tmsh then LTM and
click on show /ltm virtual toward the bottom

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>e.     <[endif]>Under Files >> config you can view
the bigip.conf file and see the command lines you used for you build

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                      i.    
<[endif]>All of the log files are here too

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>f.      <[endif]>Feel free to just poke around

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Troubleshoot using TCPDump or Curl.

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo32">

<[if !supportLists]>1.     <[endif]>Go to your www\_vs (10.1.10.100)
virtual server and set Source Address Translation to None.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo32">

<[if !supportLists]>a.     <[endif]>Now browse the web site.  You will
not be able to access it even though the status of the virtual is
available.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo32">

<[if !supportLists]>                                      i.    
<[endif]>Because the BIG-IP is not the server’s default gateway of the
servers their response goes around the BIG-IP.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>b.     <[endif]>The web administrator tells you
everything is fine as far as he can see and thinks the issue is with the
BIG-IP, because they ALWAYS think the issue is with the BIG-IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>c.      <[endif]>You begin by debugging the client
connections to the web servers through the BIG-IP using TCPDump

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo30">

<[if !supportLists]>2.     <[endif]>SSH to the management port of your
BIG-IP. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

Remember the BIG-IP is a full proxy.  You will need two dumps and
therefore two SSH windows for the client-side connection and the
server-side connection.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.25in;mso-add-space:
   auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>a.     <[endif]>First let’s see if we are hitting
the virtual server.  At the Linux CLI prompt:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo30">

<[if !supportLists]>                                      i.    
<[endif]>tcpdump –i <client vlan name> host –X –s128 10.1.10.100 and
port 80

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo30">

<[if !supportLists]>1.     <[endif]>This is a little overkill, but a
good example of syntax.  We will only look at traffic headed for the
virtual server. We will see the first 128 bytes (-s128) in ASCII (-X).

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>b.     <[endif]>Go to your browser and attempt to
access the virtual server.  You should see something like this:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

17:38:40.051122 IP 10.1.10.1.43932 > 10.1.10.245.http: S
522853636:522853636(0) win 8192 <mss 1460,nop,wscale 2,nop,nop,sackOK>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0000:  0ffe 0800 4500 0034 0a40 4000 4006 0699 
....E..4.@@.@...

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0010:  0a80 0a01 0a80 0aeb ab9c 0050 1f2a 1d04 
...........P.\*..

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0020:  0000 0000 8002 2000 3d10 0000 0204 05b4 
........=.......

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0030:  0103 0302 0101 0402                      ........

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

17:38:40.051169 IP 10.1.10.245.http > 10.1.10.1.43932: S
245310500:245310500(0) ack 522853637 win 4380 <mss 1460,sackOK,eol>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0000:  0ffe 0800 4500 0030 27ef 4000 ff06 29ed 
....E..0'.@...).

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0010:  0a80 0aeb 0a80 0a01 0050 ab9c 0e9f 2424 
.........P....$$

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0020:  1f2a 1d05 7012 111c 2a0e 0000 0204 05b4 
.\ *..p...*.......

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0030:  0402 0000                                ....

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

17:38:40.053644 IP 10.1.10.1.43932 > 10.1.10.244.http: . ack 1 win 64240

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0000:  0ffe 0800 4500 0028 0a41 4000 4006 06a4 
....E..(.A@.@...

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0010:  0a80 0a01 0a80 0aeb ab9c 0050 1f2a 1d05 
...........P.\*..

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0020:  0e9f 2425 5010 faf0 7018 0000            ..$%P...p...

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

17:38:40.053648 IP 10.1.10.1.43932 > 10.1.10.245.http: P 1:416(415) ack
1 win 64240

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0000:  0ffe 0800 4500 01c7 0a42 4000 4006 0504 
....E....B@.@...

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0010:  0a80 0a01 0a80 0aeb ab9c 0050 1f2a 1d05 
...........P.\*..

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0020:  0e9f 2425 5018 faf0 43c5 0000 4745 5420
 ..$%P...C...GET.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0030:  2f20 4854 5450 2f31 2e31 0d0a 486f 7374 
/.HTTP/1.1..Host

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.75in">

        0x0040:  3a20 3130 2e31 3238 2e31 302e 3233 350d  :.10.1.10.245.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>c.      <[endif]>Well you are hitting the virtual
server so let’s look a little deeper and expand our dump.  Your original
client IP is in the first line of the dump 16:44:58.801250 IP
10.1.10.1.41536 > 10.128.10.245.https

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo30">

<[if !supportLists]>3.     <[endif]>In the second SSH window we will do
an expanded tcpdump for the sake of interest

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>a.     <[endif]>tcpdump –i <server vlan name> -X
–s128 host <client IP>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>b.     <[endif]>Hit your virtual server again.  As
you can see, we are sending packers to the pool members.  They just
aren’t responding so we can reasonably suspect it’s a server issue. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo30">

<[if !supportLists]>4.     <[endif]>It could be a port issue.  Let’s
check to see if the server is responding on port 80.  On the BIG-IP, in
an SSH window:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>a.     <[endif]>Do a <ctrl-c> to escape out of
tcpdump, if you are still in it, and use curl to test the server

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo30">

<[if !supportLists]>                                      i.    
<[endif]>curl –i <server ip>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo30">

<[if !supportLists]>1.     <[endif]>“-i” to dump the HTTP header
information also

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

[root@bigip249:Active:Standalone] config # curl -i 10.1.20.11

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

HTTP/1.1 200 OK

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

Date: Sat, 26 Jul 2014 19:25:28 GMT

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

Server: Apache/2.2.22 (Ubuntu)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

X-Powered-By: PHP/5.4.9-4ubuntu2.2

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

Vary: Accept-Encoding

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

Content-Length: 3819

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

Connection: close

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

Content-Type: text/html

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

<html>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

<head>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

<TITLE>Using virtual server 10.1.20.11 and pool member 10.1.20.11 (Node
#1)</TITLE>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.75in">

<meta http-equiv="Content-Type" content="text/html; charset=us-ascii" />

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo30">

<[if !supportLists]>b.     <[endif]>The server is responding to the
BIG-IP when directly connected, but not through the virtual server. 
Sounds like the server is routing around the BIG-IP, which means the
BIG-IP is not the default gateway.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51">

Turn SNAT Automap back on the www\_vs virtual server

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <h1>

Lab 8: Device Service Clusters (DSC)

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

We want to familiarize you with the concept of Device and Traffic Groups
as well as the building of Active-Standby, Active-Active BIG-IP pairs. 
While there is a wizard, for this lab, configuration will be done
manually.  The wizard will only build A/S HA groups. In order to build
Active-Active and beyond a pair you will need to know the four steps to
add a device object to a cluster. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Base Networking and HA VLAN

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal" style="margin-top:12.0pt">

You will be creating a high availability cluster using the second BIG-IP
(bigip2) in your lab, so let’s prep our current BIG-IP and create a high
availability VLAN.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo20">

<[if !supportLists]>1.     <[endif]>On BigIpA.f5agility.com archive your
configuration in case you need to revert

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>Go to System >> Archives and create
a new archive.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>b.     <[endif]>You will be using your third
interface (1.3) for Network Failover and ConfigSync.  This requires
certain ports to be open on the Self IP; TCP port 4353 for ConfigSync,
TCP port 1026 for Network Failover and TCP port 6699 for the Master
Control Program.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                      i.    
<[endif]>Build a new untagged VLAN ha\_vlan on interface 1.3

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo27">

<[if !supportLists]>                                     ii.    
<[endif]>Add a self-IP address to the VLAN, 192.168.20.1 net mask
255.255.255.0.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo27">

<[if !supportLists]>1.     <[endif]>Under Port Lockdown, select Allow
Default, to open ports required for HA communications.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:189.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo27">

<[if !supportLists]>2.     <[endif]>Go to https://10.1.1.246 which is
BigIpB.f5agility.com and login.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>a.     <[endif]>Bigip102 has already been licensed
and provision.  You will need to set up the base networking.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0" style="margin-left:.5in;border-collapse:collapse;border:none;mso-border-alt:
    solid black .5pt;mso-yfti-tbllook:1184;mso-padding-alt:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <tr style="mso-yfti-irow:0;mso-yfti-firstrow:yes">

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border:solid black 1.0pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

Interface

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border:solid black 1.0pt;
     border-left:none;mso-border-left-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

Untagged VLAN

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border:solid black 1.0pt;
     border-left:none;mso-border-left-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

Self IP

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border:solid black 1.0pt;
     border-left:none;mso-border-left-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

Netmask

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr style="mso-yfti-irow:1">

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border:solid black 1.0pt;
     border-top:none;mso-border-top-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

1.1

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

client\_vlan

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

10.1.10.246

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

255.255.255.0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr style="mso-yfti-irow:2">

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border:solid black 1.0pt;
     border-top:none;mso-border-top-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

1.2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

server\_vlan

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

10.1.20.246

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

255.255.255.0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr style="mso-yfti-irow:3;mso-yfti-lastrow:yes">

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border:solid black 1.0pt;
     border-top:none;mso-border-top-alt:solid black .5pt;mso-border-alt:solid black .5pt;
     padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

1.3

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.85pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

ha\_vlan

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

192.168.20.2

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td width="180" valign="top" style="width:134.9pt;border-top:none;border-left:
     none;border-bottom:solid black 1.0pt;border-right:solid black 1.0pt;
     mso-border-top-alt:solid black .5pt;mso-border-left-alt:solid black .5pt;
     mso-border-alt:solid black .5pt;padding:0in 5.4pt 0in 5.4pt">

.. raw:: html

   <p class="MsoNormal">

255.255.255.0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </table>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>b.     <[endif]>Set Port Lockdown to Allow Default

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>c.      <[endif]>Build the default gateway
destination 0.0.0.0, mask 0.0.0.0, gateway ip address 10.128.10.1

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo27">

<[if !supportLists]>d.     <[endif]>What is the status your BIG-IPs? 
Check the upper left-hand corner next to the F5 ball. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Configure HA

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l7 level1 lfo45">

<[if !supportLists]>1.     <[endif]>On each BIG-IP, prior to building
the Device Trust, it is recommended to renew the BIG-IP self-signed
certificate with valid information and regenerate the local Device Trust
certificate

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l15 level1 lfo46">

<[if !supportLists]>a.     <[endif]>Under System >> Certificate
Management >> Device Certificate Management >> Device Certificate,
select the Renew… button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Common Name: <the Hostname of the BIG-IP in the upper left
corner>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Country: United States       (or your country of preference)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Lifetime: 3650

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>Lifetime is important.  If your cert
expires your HA setup will fail

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>Select Finished.  Your browser will ask to exchange certs with
the BIG-IP again

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l15 level1 lfo46">

<[if !supportLists]>b.     <[endif]>Under Device Management >> Device
Trust >> Local Domain select Reset Device Trust…

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l18 level1 lfo47">

<[if !supportLists]>                                      i.    
<[endif]>In the Certificate Signing Authority select Generate New
Self-Signed Authority and hit Update

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l7 level1 lfo45">

<[if !supportLists]>2.     <[endif]>On each BIG-IP configure the device
object failover parameters the BIG-IP will send to other BIG-IPs that
want to be a part of a sync-only or sync-failover group

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level2 lfo45">

<[if !supportLists]>a.     <[endif]>Under Device Management >> Devices,
select the local BIG-IP.  It will have the (Self) suffix.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l7 level3 lfo45">

<[if !supportLists]>                                      i.    
<[endif]>Under Device Connectivity on the top bar select:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level4 lfo45">

<[if !supportLists]>1.     <[endif]>ConfigSync

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level5 lfo45">

<[if !supportLists]>a.     <[endif]>Use the Self IP address of the HA
VLAN for your Local Address.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l7 level3 lfo45">

<[if !supportLists]>                                     ii.    
<[endif]>Failover Network

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>In the Failover Unicast
Configuration section select the Add button

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>2.     <[endif]>Use the Self IP address the HA VLAN
for your Address

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>3.     <[endif]>Leave the Port at the default
setting of 1026

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>4.     <[endif]>Note: Multicast is for Viprion
chassis’ only

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     v.    
<[endif]>Mirroring

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>Primary Local Mirror Address: use
the Self IP address of the HA VLAN for your

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>2.     <[endif]>Secondary Local Mirror Address: None

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>3.     <[endif]>On bigip01.f5agility.com build the
Device Trust.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Under Device Management >> Device
Trust >> Device Trust Members and select Add to add other BIG-IP(s) you
will trust.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Device IP Address: <management IP address of the BIG-IP to add>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>You could use any Self IP if the
out-of-band management interface is not configured.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Enter the Administrator Username and Password of the BIG-IP you
are trusting

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Select Retrieve Device Information

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>The certificate information and name
from the other BIG-IP should appear

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>Select Device Certificate Matches to proceed

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     v.    
<[endif]>Select Add Device

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>On each BIG-IP check the other
BIG-IP in the Device Trust Members list.  Is all the information there?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:99.0pt">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraph" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    vi.    
<[endif]>If some information is missing delete the trust and try again

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:99.0pt">

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                  vii.    
<[endif]>What are the statuses of your BIG-IPs now?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-top:12.0pt;margin-right:0in;
   margin-bottom:0in;margin-left:1.75in;margin-bottom:.0001pt;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>They should be In Sync.  But wait! 
Although they show in sync, only a Sync-Only group was created.  We now
need to create a Sync-Failover group to facilitate failover.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-top:12.0pt;margin-right:0in;
   margin-bottom:0in;margin-left:1.75in;margin-bottom:.0001pt;mso-add-space:auto">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-top:12.0pt;margin-right:0in;
   margin-bottom:0in;margin-left:.25in;margin-bottom:.0001pt;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>4.     <[endif]>On BigIpA.f5agility.com create a new
Sync-Failover device group

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-top:12.0pt;margin-right:0in;
   margin-bottom:0in;margin-left:.75in;margin-bottom:.0001pt;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>Under Device Management >> Device
Group create a new device group

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Name: my-device-group

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Group Type: Sync-Failover

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Add the members of the group to the Includes box

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>Check the Network Failover setting for the group

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>Check Device Groups on each BIG-IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     v.    
<[endif]>Did you have to create the Device Group on the other BIG-IP?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>Is the full configuration
synchronized yet?   (No! Only the Device Group is sync’d)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    vi.    
<[endif]>What is your sync status?  

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>It should be Awaiting Initial Sync

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                  vii.    
<[endif]>Click on the sync status or go to Device Management >> Overview
(or click on Awaiting Initial Sync) of the BIG-IP with the good/current
configuration

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                 viii.    
<[endif]>Click the device with the configuration you want to
synchronize.  Sync Options should appear.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    ix.    
<[endif]>Synchronize to Group.  It could take up to 30 seconds for
synchronization to complete.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>NOTE: During the Awaiting Initial
Sync phase either BIG-IP can perform the synchronization and the other
BIG-IP will be overwritten.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>2.     <[endif]>What are the statuses of your
BIG-IPs?   Do you have an active-standby pair?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>3.     <[endif]>Are the configurations the same?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>5.     <[endif]>Now that you have created your HA
environment, HA selections will show up for SNAT addressed (not tied to
your base network), persistence profiles and connection mirroring on
virtual servers.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>a.     <[endif]>Go to your Active BIG-IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>b.     <[endif]>Go to your persistence profile
my-src-persistence and check the Mirror Persistence box

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>c.      <[endif]>Go to your www\_vs virtual server
and set the Default Persistence Profile to my-src-persistence

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>d.     <[endif]>Synchronize your changes.   Did the
changes sync?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>e.     <[endif]>On each BIG-IP go to Module
Statistics > Local Traffic and bring up the persistence record
statistics

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo33">

<[if !supportLists]>                                      i.    
<[endif]>Go to the home page of your www\_vs web service
(http://10.1.10.100).  Refresh a few times.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo33">

<[if !supportLists]>                                     ii.    
<[endif]>Check the persistence records on each of your BIG-IPs, you
should see the records are mirrored on each device

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:1.5in">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo33">

<[if !supportLists]>6.     <[endif]>Go to Device Management >> Traffic
Groups.  As you can see the default traffic group “traffic-group-1”
already exists.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>a.     <[endif]>Select traffic-group-1.  Check out
the page information and then select Force to Standby. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>b.     <[endif]>What are the statuses of your
BIG-IPs?  Go to your web page.   What is the client IP?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>c.      <[endif]>Go to your self-IP addresses.  What
traffic group are they in?  What does it mean?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo33">

<[if !supportLists]>d.     <[endif]>Archive your work.

.. raw:: html

   </p>

.. raw:: html

   <h1>

Bonus Lab – Traffic groups, iApps and Active-Active

.. raw:: html

   </h1>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

If you have time, this is a bonus lab.  Here you will create a new
traffic group.  You will use iApps to create a new HTTP application that
reside in that address group and you will create a floating IP address
that will be used as the default gateway that also resides in that
traffic group.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Building a new traffic group and floating IP.

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l23 level1 lfo48">

<[if !supportLists]>1.     <[endif]>On your Active BIG-IP, go to Device
Management >> Traffic Groups and hit Create

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l23 level2 lfo48">

<[if !supportLists]>a.     <[endif]>Use the f5.http template, which was
designed for general web services

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                      i.    
<[endif]>Name: iapp\_tg

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     ii.    
<[endif]>Take the defaults for the rest.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l23 level1 lfo48">

<[if !supportLists]>2.     <[endif]>Add a floating Self-IP to the
server\_vlan.  Go to Network >> Self IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level2 lfo45">

<[if !supportLists]>b.     <[endif]>Name: server\_gateway

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level2 lfo45">

<[if !supportLists]>c.      <[endif]>IP Address:10.1.20.240

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level2 lfo45">

<[if !supportLists]>d.     <[endif]>Netmask: 255.255.255.0

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l7 level2 lfo45">

<[if !supportLists]>e.     <[endif]>VLAN/Tunnel: server\_vlan

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l7 level2 lfo45">

<[if !supportLists]>f.      <[endif]>Traffic Group: iapp\_tg (floating)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in">

.. raw:: html

   <h3 style="margin-left:0in">

Building an HTTP application using an iApp template.

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l9 level1 lfo44">

<[if !supportLists]>1.     <[endif]>Go to iApp >> Application Services
and hit Create.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l9 level2 lfo44">

<[if !supportLists]>a.     <[endif]>Use the f5.http template, which was
designed for general web services

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                      i.    
<[endif]>Set the Template Selection to Advanced

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                     ii.    
<[endif]>Name: my\_new\_iapp

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                    iii.    
<[endif]>Traffic Group: iapp\_tg (floating)

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>1.     <[endif]>You will have to uncheck the Inherit
traffic group from current partition / path.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                    iv.    
<[endif]>Under Template Options

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l30 level1 lfo49">

<[if !supportLists]>1.     <[endif]>Select the Advanced – Configure
advanced options for the configuration mode

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                     v.    
<[endif]>Under the Network tab

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l0 level1 lfo50">

<[if !supportLists]>1.     <[endif]>How have you configured routing on
your web servers?  Servers have a route to the clients through the
BIG-IP system

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>a.     <[endif]>In other words, the BIG-IP is the
default gateway for the servers

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>b.     <[endif]>Otherwise the template would use
SNAT by default

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                    vi.    
<[endif]>Under Virtual Server and Pools

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l19 level1 lfo51">

<[if !supportLists]>1.     <[endif]>Your virtual server IP is
10.1.10.110

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l19 level1 lfo51">

<[if !supportLists]>2.     <[endif]>Your hostname will be
www.f5agility.com because you have to put one in.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l19 level1 lfo51">

<[if !supportLists]>3.     <[endif]>Create a new pool with the members
10.1.20.14:80 and 10.1.20.15:80

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:2.25in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level5 lfo17">

<[if !supportLists]>c.      <[endif]>If you hit add after the last pool
member and have a new row, you will need to delete the row prior to
finishing

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                  vii.    
<[endif]>Hit Finished at the bottom of the page

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l9 level1 lfo44">

<[if !supportLists]>2.     <[endif]>Go to iApp >> Application Services
and select the new application you created

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l9 level2 lfo44">

<[if !supportLists]>a.     <[endif]>Select Components from the top bar

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                      i.    
<[endif]>Here you will see all the configuration items created by the
iApp

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l9 level3 lfo44">

<[if !supportLists]>                                     ii.    
<[endif]>Do you see anything created that you weren’t asked about?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l9 level1 lfo44">

<[if !supportLists]>3.     <[endif]>Remember the concept of strictness? 
Let’s test that out\`

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l1 level1 lfo52">

<[if !supportLists]>a.     <[endif]>Go to Local Traffic >> Pools >> Pool
List

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l26 level1 lfo53">

<[if !supportLists]>                                      i.    
<[endif]>Select the pool created by your iApp: my\_new\_iapp\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l26 level1 lfo53">

<[if !supportLists]>                                     ii.    
<[endif]>Attempt to add 10.15.11.13:80 to your my\_new\_iapp\_pool

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>2.     <[endif]>Did it fail?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l1 level1 lfo52">

<[if !supportLists]>b.     <[endif]>Go to your iApp and select
Reconfigure from the top bar

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l29 level1 lfo54">

<[if !supportLists]>                                      i.    
<[endif]>Now attempt to add your new pool member

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l29 level1 lfo54">

<[if !supportLists]>                                     ii.    
<[endif]>You can check the Components tab to verify your success

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:solid windowtext 1.0pt;
   mso-border-alt:solid windowtext .5pt;padding:1.0pt 4.0pt 1.0pt 4.0pt;
   background:#FDE9D9;mso-background-themecolor:accent6;mso-background-themetint:
   51;margin-left:.15in;margin-right:1.05in">

.. raw:: html

   <p class="CallOut" style="margin-top:9.0pt;margin-right:0in;margin-bottom:9.0pt;
   margin-left:.6in;background:#FDE9D9;mso-background-themecolor:accent6;
   mso-background-themetint:51">

SYNCHRONIZE YOUR CHANGES

.. raw:: html

   </p>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

Active-Active Setup

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo21">

<[if !supportLists]>1.     <[endif]>Now, let’s make our sync-failover
group active-active.  On the Active BIG-IP:

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo21">

<[if !supportLists]>a.     <[endif]>Go to Device Management >> Traffic
Groups

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo21">

<[if !supportLists]>                                      i.    
<[endif]>Go to you iapp\_tg traffic group. 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo21">

<[if !supportLists]>                                     ii.    
<[endif]>Under Advanced Setup Options

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo21">

<[if !supportLists]>1.     <[endif]>You are going to set up iapp\_tg to
prefer to run on bigip02.f5agility.com and auto failback to bigip02 if
bigip02 should go down and come back up later.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level4 lfo17">

<[if !supportLists]>2.     <[endif]>Is this normally a good idea?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iii.    
<[endif]>Failover Method: HA Order

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    iv.    
<[endif]>Auto Failback: <checked>

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:1.25in;mso-add-space:
   auto;text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                     v.    
<[endif]>Failover Order: bigip102.f5agility.com then
bigip01.f5agility.com

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:1.25in;mso-add-space:auto;
   text-indent:-1.25in;mso-text-indent-alt:-9.0pt;mso-list:l22 level3 lfo17">

<[if !supportLists]>                                    vi.    
<[endif]>Ensure you synchronized the change to the other BIG-IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-left:81.0pt">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpFirst" style="margin-left:.25in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level1 lfo17">

<[if !supportLists]>2.     <[endif]>If the traffic group is active on
the wrong BIG-IP initially you will have to do a Force to Standby on the
traffic group to make it active on the BIG-IP you want it on by default

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>a.     <[endif]>What is the ONLINE status of each of
your BIG-IPs?

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpMiddle" style="margin-left:.75in;mso-add-space:
   auto;text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>b.     <[endif]>Reboot the BIG-IP with your second
traffic group on it.   Watch to see if the application becomes active on
the other BIG-IP during the reboot and if it falls back to the Default
Device once the BIG-IP has come back up.

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoListParagraphCxSpLast" style="margin-left:.75in;mso-add-space:auto;
   text-indent:-.25in;mso-list:l22 level2 lfo17">

<[if !supportLists]>c.      <[endif]>You can verify this by checking
your traffic groups or going to the web server and looking at the client
IP

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal" style="margin-top:0in">

 

.. raw:: html

   </p>

.. raw:: html

   <h1>

Appendix

.. raw:: html

   </h1>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

BIG-IP Policy for retrieving jpeg images from the image\_pool

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   <p class="MsoNormal">

 

.. raw:: html

   </p>

.. raw:: html

   <p class="MsoNormal">

.. raw:: html

   </p>

.. raw:: html

   <div
   style="mso-element:para-border-div;border:none;border-top:solid windowtext 1.5pt;
   padding:1.0pt 0in 0in 0in;margin-left:4.5pt;margin-right:0in">

.. raw:: html

   <h3 style="margin-left:0in">

 

.. raw:: html

   </h3>

.. raw:: html

   </div>

.. raw:: html

   </div>

.. raw:: html

   </body>

.. raw:: html

   </html>
