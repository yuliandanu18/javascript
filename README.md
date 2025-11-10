# javascript


for grab or download socmed like FB comment 

F12
then paste

(function() {
  const html = document.documentElement.outerHTML;
  const blob = new Blob([html], { type: "text/html" });
  const a = document.createElement("a");
  a.href = URL.createObjectURL(blob);
  a.download = document.title.replace(/[^\w\s]/gi, '_') + ".html";
  a.click();
})();
