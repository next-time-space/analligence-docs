<!DOCTYPE html>
<html lang="en">
  <head>
  
  <style>
  .accordian {
  position: absolute;
    bottom: 60px;
  }
  </style>
  	<link rel='stylesheet' href='/analligence/stylesheets/kernal.css' />
    {{#metricPage}}
    <link rel='stylesheet' href='/analligence/stylesheets/nv.d3.min.css' />
    {{/metricPage}}
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta name="description" content="Free open source analitics bussiness tool to find customer engegment. Create catalogs, segment, see metrics and make decision based on analytics metrics.">
	<meta http-equiv="content-type" content="text/html;charset=UTF-8">
	<meta property="og:title" content="Free Open source business analitics tool" />
	<meta property="og:url" content="https://analligence.nexttimespace.com" />
	<meta property="og:type" content="website" />
	<meta property="og:description" content="Involve artificial intelligence in analytics. Create catalogs, segment, see metrics and make decision based on analytics metrics." />
	<meta property="og:image" content="https://analligence.nexttimespace.com/images/appLogo.png" />
	<title>Next Time Space Analligence</title>
	
	<script>window.wslist = [{{#ws}}'{{.}}',{{/ws}}]</script>
  <style>
  table tbody tr:hover td {
background-color: red;
}
  </style>
  </head>
  <body style="height: 100vh">
  <div id="cover"></div>
  <div id="dashboard1" style="height: 100%" class="maincontent">
   <nav class="headerMainBar navbar navbar-expand-md navbar-dark bg-dark">
  <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <a class="navbar-brand" href="/analligence/main-menu">
  <img  src="/analligence/images/appLogo.png" width="155" height="40" alt="Next Time Space">
  </a>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active">
        <div class="dropdown nav-link">
  <button class="button bigDropDown dropdown-toggle" type="button" id="workspaceButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
   ...
  </button>
  <div class="dropdown-menu bigDropDown" id="headerWorkspaceList" aria-labelledby="dropdownMenuButton">
  {{#ws}}
    <a class="dropdown-item  " href="/analligence/cats/list?workspace={{.}}">{{.}}</a>
    {{/ws}}
  </div>
</div>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="/analligence/workspace">Work spaces</a>
      </li>
      
    </ul>
   <img alt="Account" src="/analligence/images/person.svg">
  </div>
</nav>

<div style=" height: 100%" class="row">
<div style="border-right: 1px solid #ccc; padding-right:0px; height: 100%" class="col-md-2 bg-dark">
<a class="sideMenuLink" href="/analligence/workspace"><div class="col-md-12 sideMenu"><img width=32 height=32 alt="" src="/analligence/images/briefcase.svg"/><span class="sideMenuTitle">&nbsp;&nbsp;Workspace</span></div></a>
<a class="sideMenuLink" href="/analligence/cats/list" kid="/analligence/cat-eng-edit"><div class="col-md-12 sideMenu"><img width=32 height=32 alt="" src="/analligence/images/book.svg"/><span class="sideMenuTitle">&nbsp;&nbsp; Catalogs</span></div></a>
<a class="sideMenuLink" href="/analligence/build"><div class="col-md-12 sideMenu" ><img width=32 height=32 alt="" src="/analligence/images/project.svg"/><span class="sideMenuTitle">&nbsp;&nbsp;Build Space</span></div></a>
<a class="sideMenuLink" href="/analligence/testspace"><div class="col-md-12 sideMenu" ><img width=32 height=32 alt="" src="/analligence/images/bug.svg"/><span class="sideMenuTitle">&nbsp;&nbsp;Test Space</span></div></a>
<a class="sideMenuLink" href="/analligence/deployspace"><div class="col-md-12 sideMenu" ><img width=32 height=32 alt="" src="/analligence/images/circuit-board.svg"/><span class="sideMenuTitle">&nbsp;&nbsp;Deploy Space</span></div></a>
<a class="sideMenuLink" href="/analligence/trends"><div class="col-md-12 sideMenu" ><img width=32 height=32 alt="" src="/analligence/images/graph.svg"/><span class="sideMenuTitle">&nbsp;&nbsp;Trends Space</span></div></a>
<a onclick="javascript:utility.hideSideMenuTitle();" class="sideMenuLink accordian" href="javascript:void(0);"><div class="col-md-12 sideMenu" ><img width=28 height=28 alt="" src="/analligence/images/chevron-left.svg"/></div></a>
</div>
<div class="col-md-10" style="padding-left: 0px">
