---
title: "publications"
bg: grey
color: black
style: left
fa-icon: files-o
---
<script>
function load_home (e) {
   (e || window.event).preventDefault();
   var con = document.getElementById('content-bib')
   ,   xhr = new XMLHttpRequest();

   xhr.onreadystatechange = function (e) { 
    if (xhr.readyState == 4 && xhr.status == 200) {
     con.innerHTML = xhr.responseText;
    }
   }

 xhr.open("GET", "http://bibbase.org/show?bib=http%3A%2F%2Fcap-csail.github.io%2F%2Ffiles%2Fcap_pubs.bib&msg=embed", true);
 xhr.setRequestHeader('Content-type', 'text/html');
 xhr.send();
}
</script>


## Publications

<div id="content-bib">
</div>
<!-- <iframe src="http://bibbase.org/show?bib=http%3A%2F%2Fcap-csail.github.io%2F%2Ffiles%2Fcap_pubs.bib&msg=embed" width="100%"  height="1500" ></iframe> -->
