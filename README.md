# FastDomParse-java

fast dom parse for java  
GitHub Pages: https://github.com/fengshangbin/FastDomParse-java

# 如何使用 FastDomParse-java
导入fastdomparse.jar
```
FastDom dom = new FastDom(htmlString)

//单目标查询
Element element = dom.querySelector("div.page li[name=1]");

//多目标查询
ArrayList<Element> elements = dom.querySelectorAll("div.page li");

//目标子查询
Element sun = element.querySelector("div.page li[name=1]");
ArrayList<Element> suns = element.querySelectorAll("div.page li[name=1]");

//element属性
String inner = element.getInnerHTML();
element.setInnerHTML("hello fast dom parse");

String outer = element.getOuterHTML();
element.setOuterHTML("<div>hello fast dom parse<div>");

String attr = element.getAttribute("id");
element.setAttribute("id", "content");
boolean hasID = element.hasAttribute("id");

//获取整个dom内容
dom.getHTML()
```

熟悉的味道，一样的配方，和原生 DOM 一样的语法，无需新学习，使用简单。
