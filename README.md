# Confluence
Confluence related items.

# Snippets
## Expand All/Collapse All UI Expand

```html
<input type="button" onclick="expandAll();" value="Expand All"/>
<input type="button" onclick="collapseAll();" value="Collapse All"/>
<script type="text/javascript">
	function expandAll(){
		$("div.rwui_expandable_item").not(".rw_open").find("a.rwui_expand").trigger('click');
		$("div.rwui_expandable_item").not(".rw_open").find("a.rwui_expand").trigger('click');		
		$("div.rwui_expandable_item").not(".rw_open").find("a.rwui_expand").trigger('click');		
	}
	function collapseAll(){
		$("div.rwui_expandable_item.rw_open").find("a.rwui_expand").trigger('click');
	}
</script>
```


## No Border for Tables Inside UI Expand
```css
<style>
div.rwui_expandable_item_body.rwui_body table.confluenceTable tbody tr td {
	border-width: 0px !important;
	background-color: rgb(243, 243, 243) !important;
}
</style>
```

## Open All Links New Tab

```javascript
<script>
jQuery(document).ready(function() {
    jQuery(".wiki-content a").attr("target", "_blank");
});
</script>
```
## Back to Top Link

```javascript
<script>AJS.$('#main-content').after('<div><a style="position:fixed;bottom:20px;right: 20px;" onClick="window.scrollTo(0, 0);">Back to Top</a></div>');</script>
```
