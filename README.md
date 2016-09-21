# ichabot for JOMBLO AGC 2.2 (blogspot).
# is supplement for auto random greeting and footer at the end of blog article. 
# this bot if special for adult indonesian blog.
# compatible with all blogspot template.
# the full code is below (injected somewhere at "<data:post.body/>" on your template):

<!--X1-->
<script type='text/javascript'>
//<![CDATA[
var relatedTitles = new Array(); var relatedTitlesNum = 0; var relatedUrls = new Array(); function related_results_labels(json){for(var i=0;i < json.feed.entry.length;i++){var entry=json.feed.entry[i]; relatedTitles[relatedTitlesNum]=entry.title.$t;for(var k=0; k < entry.link.length; k++) {if(entry.link[k].rel == 'alternate'){relatedUrls[relatedTitlesNum]=entry.link[k].href;relatedTitlesNum++;break;}}}}function removeRelatedDuplicates(){var tmp=new Array(0);var tmp2=new Array(0);for(var i=0;i < relatedUrls.length;i++){if(!contains(tmp, relatedUrls[i])){tmp.length += 1;tmp[tmp.length - 1]=relatedUrls[i];tmp2.length += 1;tmp2[tmp2.length - 1]=relatedTitles[i];}}relatedTitles=tmp2; relatedUrls=tmp;}function contains(a,e){for(var j=0;j < a.length;j++)if(a[j]==e)return true;return false;}function printRelatedLabels(){var r=Math.floor((relatedTitles.length - 1) * Math.random()); var i = 0; document.write('<ul>'); while (i < relatedTitles.length && i < 20){document.write('<li><a href="' + relatedUrls[r] + '">' + relatedTitles[r] + '</a></li>');if(r < relatedTitles.length - 1){r++;}else{r=0;}i++;} document.write('</ul>');}
//]]>
</script>
<b><data:blog.pageName/>
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/kota.js'></script><div style='display:none;'>.</div>
</b> - 
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/ab.js'></script><div style='display:none;'>.</div>
 <a expr:href='data:blog.homepageUrl'><data:blog.title/></a> 
<script src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/cd.js'></script><div style='display:none;'>.</div>
 <data:blog.pageName/>, 
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/ef.js'></script><div style='display:none;'>.</div>
<b:loop values='data:post.labels' var='label'> <a expr:href='data:label.url' rel='dofollow'>kategori <data:label.name/></a>,</b:loop>
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/yz.js'></script><div style='display:none;'>.</div>
<br/><br/>Keterangan <br/>
Judul : <span itemprop='itemreviewed'><b><data:post.title/></b></span><br/>Tautan : <a expr:href='data:post.url'><data:post.title/></a><br/>
<script>document.write(unescape(&#39;%3C%69%66%72%61%6D%65%20%73%72%63%3D%22%2F%2F%61%64%73%2E%65%78%6F%63%6C%69%63%6B%2E%63%6F%6D%2F%69%66%72%61%6D%65%2E%70%68%70%3F%69%64%7A%6F%6E%65%3D%32%32%33%30%39%32%39%26%73%69%7A%65%3D%37%32%38%78%39%30%22%20%77%69%64%74%68%3D%22%37%32%38%22%20%68%65%69%67%68%74%3D%22%39%30%22%20%73%63%72%6F%6C%6C%69%6E%67%3D%22%6E%6F%22%20%6D%61%72%67%69%6E%77%69%64%74%68%3D%22%30%22%20%6D%61%72%67%69%6E%68%65%69%67%68%74%3D%22%30%22%20%66%72%61%6D%65%62%6F%72%64%65%72%3D%22%30%22%3E%3C%2F%69%66%72%61%6D%65%3E&#39;));</script>
<br/><br/>
<!--end of X1-->
                            <data:post.body/>
<!--X2-->
<b:if cond='data:blog.pageType == &quot;item&quot;'><div><div><span><br/><br/>
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/rp.js'></script><div style='display:none;'>.</div>
 <data:blog.pageName/> 
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/sq.js'></script><div style='display:none;'>.</div>
 </span></div></div><b:else/><p><data:post.body/></p>
</b:if>
<b:if cond='data:blog.pageType == &quot;item&quot;'><div><br/>
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/tn.js'></script><div style='display:none;'>.</div>
 <strong><u><data:blog.pageName/></u></strong>
<script type='text/javascript' src='https://cdn.rawgit.com/ichamasdiya/ichabot/master/uo.js'></script><div style='display:none;'>.</div>
 <strong><data:post.url/></strong></div><br/><b:else/>
</b:if>
<!--end of X2-->
