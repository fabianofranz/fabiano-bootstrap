$(document).ready(function() {
	DD_roundies.addRule(".rounded", "6px", false);
	DD_roundies.addRule("button", "6px", false);
	DD_roundies.addRule("div.box", "6px", false);
	DD_roundies.addRule("a.button", "6px", false);
	DD_roundies.addRule("ul.dropdown-menu > li:hover", "6px", false);
	DD_roundies.addRule("ul.dropdown-menu li ul li:hover a", "6px", false);
	$(".gradient").gradient({from: "ffffff", to: "A7D8E9", direction: "horizontal"});
	$("input.autoclean, textarea.autoclean").focus(function() { $(this).val(""); });
	$("label.required").append("<span class=\"required\">*</span>");
	jQuery(function($) { $(".date").mask("99/99/9999"); });
	jQuery(function($) { $(".time").mask("99:99"); });
	jQuery(function($) { $(".numeric").numeric(); });
	$("form").submit(function() { 
		$("button", this).attr("disabled", "disabled").addClass("disabled");
    	$("<img src=\"images/ajax-loading-inline.gif\" />").insertAfter("button:last", this);
	});
	$("a.tooltip").qtip({
		show: "mouseover",
		hide: "mouseout",
		content: $(this).attr("alt"),
		position: {
			corner: { target: "topMiddle", tooltip: "bottomMiddle" }
		},
		style: { name: "dark", tip: "bottomMiddle", border: { width: 7, radius: 5 } }
	});
	$("a[href='http://google.com']").colorbox({width:"80%", height:"80%", iframe:true});
	$("a[href='internal.html']").colorbox({width:"300px", height:"300px", iframe:true});
	$("a[href='internal2.html']").colorbox();
	$("#inline").colorbox({width:"80%", inline:true, href:"#inline_content", title:"an inline content!"});
});

go = function(dest) { window.location.assign(dest); }

alert = function(text) { $.prompt(text, {opacity: 0.9, prefix: "modal", overlayspeed: "fast", top: "70px" }); DD_roundies.addRule("div.modal", "5px", true); }
confirm = function(text, callbackFunction) { $.prompt(text, { buttons: { Ok: true, Cancel: false }, opacity: 0.9, prefix: "modal", overlayspeed: "fast", top: "70px", callback: function(v,m,f) { /*alert("value: " + v);*/ callbackFunction(v); return true; } }); DD_roundies.addRule("div.modal", "5px", true); }

String.prototype.trim = function() { return this.replace(/^\s+|\s+$/g,""); }
String.prototype.ltrim = function() { return this.replace(/^\s+/,""); }
String.prototype.rtrim = function() { return this.replace(/\s+$/,""); }
String.prototype.startsWith = function(str) { return (this.match("^"+str)==str); }
String.prototype.endsWith = function(str) { return (this.match(str+"$")==str); }
String.prototype.replaceAll = function(from, to) {
	var str = this; 
	var pos = str.indexOf(from);
	while (pos > -1){
		str = str.replace(from, to);
		pos = str.indexOf(from);
	}
	return (str);
}

