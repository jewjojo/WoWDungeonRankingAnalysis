<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>finalProject</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>




<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>



<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/*
 * Webkit scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-corner {
  background: var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-thumb {
  background: rgb(var(--jp-scrollbar-thumb-color));
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-right: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-bottom: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar */

[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-corner,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-corner {
  background-color: transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-thumb,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid transparent;
  border-right: var(--jp-scrollbar-endpad) solid transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid transparent;
  border-bottom: var(--jp-scrollbar-endpad) solid transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0px solid transparent;
  border-right: 0px solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0px solid transparent;
  border-bottom: 0px solid transparent;
}

/*
 * Phosphor
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Widget, /* </DEPRECATED> */
.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  cursor: default;
}


/* <DEPRECATED> */ .p-Widget.p-mod-hidden, /* </DEPRECATED> */
.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-CommandPalette, /* </DEPRECATED> */
.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-CommandPalette-search, /* </DEPRECATED> */
.lm-CommandPalette-search {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-content, /* </DEPRECATED> */
.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-CommandPalette-header, /* </DEPRECATED> */
.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}


/* <DEPRECATED> */ .p-CommandPalette-item, /* </DEPRECATED> */
.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}


/* <DEPRECATED> */ .p-CommandPalette-itemIcon, /* </DEPRECATED> */
.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemContent, /* </DEPRECATED> */
.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}


/* <DEPRECATED> */ .p-CommandPalette-itemShortcut, /* </DEPRECATED> */
.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemLabel, /* </DEPRECATED> */
.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
	border:1px solid transparent;
  background-color: transparent;
  position: absolute;
	z-index:1;
	right:3%;
	top: 0;
	bottom: 0;
	margin: auto;
	padding: 7px 0;
	display: none;
	vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
	content: "X";
	display: block;
	width: 15px;
	height: 15px;
	text-align: center;
	color:#000;
	font-weight: normal;
	font-size: 12px;
	cursor: pointer;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-DockPanel, /* </DEPRECATED> */
.lm-DockPanel {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-widget, /* </DEPRECATED> */
.lm-DockPanel-widget {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-tabBar, /* </DEPRECATED> */
.lm-DockPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-DockPanel-handle, /* </DEPRECATED> */
.lm-DockPanel-handle {
  z-index: 2;
}


/* <DEPRECATED> */ .p-DockPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-DockPanel-handle:after, /* </DEPRECATED> */
.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}


/* <DEPRECATED> */ .p-DockPanel-overlay, /* </DEPRECATED> */
.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}


/* <DEPRECATED> */ .p-DockPanel-overlay.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Menu, /* </DEPRECATED> */
.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-Menu-content, /* </DEPRECATED> */
.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-Menu-item, /* </DEPRECATED> */
.lm-Menu-item {
  display: table-row;
}


/* <DEPRECATED> */
.p-Menu-item.p-mod-hidden,
.p-Menu-item.p-mod-collapsed,
/* </DEPRECATED> */
.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}


/* <DEPRECATED> */
.p-Menu-itemIcon,
.p-Menu-itemSubmenuIcon,
/* </DEPRECATED> */
.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}


/* <DEPRECATED> */ .p-Menu-itemLabel, /* </DEPRECATED> */
.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}


/* <DEPRECATED> */ .p-Menu-itemShortcut, /* </DEPRECATED> */
.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-MenuBar, /* </DEPRECATED> */
.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-MenuBar-content, /* </DEPRECATED> */
.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}


/* <DEPRECATED> */ .p--MenuBar-item, /* </DEPRECATED> */
.lm-MenuBar-item {
  box-sizing: border-box;
}


/* <DEPRECATED> */
.p-MenuBar-itemIcon,
.p-MenuBar-itemLabel,
/* </DEPRECATED> */
.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-ScrollBar, /* </DEPRECATED> */
.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-ScrollBar-button, /* </DEPRECATED> */
.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-track, /* </DEPRECATED> */
.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-thumb, /* </DEPRECATED> */
.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-SplitPanel-child, /* </DEPRECATED> */
.lm-SplitPanel-child {
  z-index: 0;
}


/* <DEPRECATED> */ .p-SplitPanel-handle, /* </DEPRECATED> */
.lm-SplitPanel-handle {
  z-index: 1;
}


/* <DEPRECATED> */ .p-SplitPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-SplitPanel-handle:after, /* </DEPRECATED> */
.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabBar, /* </DEPRECATED> */
.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='horizontal'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='vertical'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}


/* <DEPRECATED> */ .p-TabBar-content, /* </DEPRECATED> */
.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='horizontal'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='vertical'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
}


/* <DEPRECATED> */
.p-TabBar-tabIcon,
.p-TabBar-tabCloseIcon,
/* </DEPRECATED> */
.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-TabBar-tabLabel, /* </DEPRECATED> */
.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}


.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing : border-box;
}


/* <DEPRECATED> */ .p-TabBar-tab.p-mod-hidden, /* </DEPRECATED> */
.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}


.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-TabBar.p-mod-dragging .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='horizontal'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='vertical'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-dragging,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing : border-box;
  background: inherit;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabPanel-tabBar, /* </DEPRECATED> */
.lm-TabPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-TabPanel-stackedPanel, /* </DEPRECATED> */
.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

@charset "UTF-8";
html{
  -webkit-box-sizing:border-box;
          box-sizing:border-box; }

*,
*::before,
*::after{
  -webkit-box-sizing:inherit;
          box-sizing:inherit; }

body{
  font-size:14px;
  font-weight:400;
  letter-spacing:0;
  line-height:1.28581;
  text-transform:none;
  color:#182026;
  font-family:-apple-system, "BlinkMacSystemFont", "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Open Sans", "Helvetica Neue", "Icons16", sans-serif; }

p{
  margin-bottom:10px;
  margin-top:0; }

small{
  font-size:12px; }

strong{
  font-weight:600; }

::-moz-selection{
  background:rgba(125, 188, 255, 0.6); }

::selection{
  background:rgba(125, 188, 255, 0.6); }
.bp3-heading{
  color:#182026;
  font-weight:600;
  margin:0 0 10px;
  padding:0; }
  .bp3-dark .bp3-heading{
    color:#f5f8fa; }

h1.bp3-heading, .bp3-running-text h1{
  font-size:36px;
  line-height:40px; }

h2.bp3-heading, .bp3-running-text h2{
  font-size:28px;
  line-height:32px; }

h3.bp3-heading, .bp3-running-text h3{
  font-size:22px;
  line-height:25px; }

h4.bp3-heading, .bp3-running-text h4{
  font-size:18px;
  line-height:21px; }

h5.bp3-heading, .bp3-running-text h5{
  font-size:16px;
  line-height:19px; }

h6.bp3-heading, .bp3-running-text h6{
  font-size:14px;
  line-height:16px; }
.bp3-ui-text{
  font-size:14px;
  font-weight:400;
  letter-spacing:0;
  line-height:1.28581;
  text-transform:none; }

.bp3-monospace-text{
  font-family:monospace;
  text-transform:none; }

.bp3-text-muted{
  color:#5c7080; }
  .bp3-dark .bp3-text-muted{
    color:#a7b6c2; }

.bp3-text-disabled{
  color:rgba(92, 112, 128, 0.6); }
  .bp3-dark .bp3-text-disabled{
    color:rgba(167, 182, 194, 0.6); }

.bp3-text-overflow-ellipsis{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal; }
.bp3-running-text{
  font-size:14px;
  line-height:1.5; }
  .bp3-running-text h1{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h1{
      color:#f5f8fa; }
  .bp3-running-text h2{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h2{
      color:#f5f8fa; }
  .bp3-running-text h3{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h3{
      color:#f5f8fa; }
  .bp3-running-text h4{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h4{
      color:#f5f8fa; }
  .bp3-running-text h5{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h5{
      color:#f5f8fa; }
  .bp3-running-text h6{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h6{
      color:#f5f8fa; }
  .bp3-running-text hr{
    border:none;
    border-bottom:1px solid rgba(16, 22, 26, 0.15);
    margin:20px 0; }
    .bp3-dark .bp3-running-text hr{
      border-color:rgba(255, 255, 255, 0.15); }
  .bp3-running-text p{
    margin:0 0 10px;
    padding:0; }

.bp3-text-large{
  font-size:16px; }

.bp3-text-small{
  font-size:12px; }
a{
  color:#106ba3;
  text-decoration:none; }
  a:hover{
    color:#106ba3;
    cursor:pointer;
    text-decoration:underline; }
  a .bp3-icon, a .bp3-icon-standard, a .bp3-icon-large{
    color:inherit; }
  a code,
  .bp3-dark a code{
    color:inherit; }
  .bp3-dark a,
  .bp3-dark a:hover{
    color:#48aff0; }
    .bp3-dark a .bp3-icon, .bp3-dark a .bp3-icon-standard, .bp3-dark a .bp3-icon-large,
    .bp3-dark a:hover .bp3-icon,
    .bp3-dark a:hover .bp3-icon-standard,
    .bp3-dark a:hover .bp3-icon-large{
      color:inherit; }
.bp3-running-text code, .bp3-code{
  font-family:monospace;
  text-transform:none;
  background:rgba(255, 255, 255, 0.7);
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
  color:#5c7080;
  font-size:smaller;
  padding:2px 5px; }
  .bp3-dark .bp3-running-text code, .bp3-running-text .bp3-dark code, .bp3-dark .bp3-code{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#a7b6c2; }
  .bp3-running-text a > code, a > .bp3-code{
    color:#137cbd; }
    .bp3-dark .bp3-running-text a > code, .bp3-running-text .bp3-dark a > code, .bp3-dark a > .bp3-code{
      color:inherit; }

.bp3-running-text pre, .bp3-code-block{
  font-family:monospace;
  text-transform:none;
  background:rgba(255, 255, 255, 0.7);
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
  color:#182026;
  display:block;
  font-size:13px;
  line-height:1.4;
  margin:10px 0;
  padding:13px 15px 12px;
  word-break:break-all;
  word-wrap:break-word; }
  .bp3-dark .bp3-running-text pre, .bp3-running-text .bp3-dark pre, .bp3-dark .bp3-code-block{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
  .bp3-running-text pre > code, .bp3-code-block > code{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:inherit;
    font-size:inherit;
    padding:0; }

.bp3-running-text kbd, .bp3-key{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#5c7080;
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  font-family:inherit;
  font-size:12px;
  height:24px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  line-height:24px;
  min-width:24px;
  padding:3px 6px;
  vertical-align:middle; }
  .bp3-running-text kbd .bp3-icon, .bp3-key .bp3-icon, .bp3-running-text kbd .bp3-icon-standard, .bp3-key .bp3-icon-standard, .bp3-running-text kbd .bp3-icon-large, .bp3-key .bp3-icon-large{
    margin-right:5px; }
  .bp3-dark .bp3-running-text kbd, .bp3-running-text .bp3-dark kbd, .bp3-dark .bp3-key{
    background:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#a7b6c2; }
.bp3-running-text blockquote, .bp3-blockquote{
  border-left:solid 4px rgba(167, 182, 194, 0.5);
  margin:0 0 10px;
  padding:0 20px; }
  .bp3-dark .bp3-running-text blockquote, .bp3-running-text .bp3-dark blockquote, .bp3-dark .bp3-blockquote{
    border-color:rgba(115, 134, 148, 0.5); }
.bp3-running-text ul,
.bp3-running-text ol, .bp3-list{
  margin:10px 0;
  padding-left:30px; }
  .bp3-running-text ul li:not(:last-child), .bp3-running-text ol li:not(:last-child), .bp3-list li:not(:last-child){
    margin-bottom:5px; }
  .bp3-running-text ul ol, .bp3-running-text ol ol, .bp3-list ol,
  .bp3-running-text ul ul,
  .bp3-running-text ol ul,
  .bp3-list ul{
    margin-top:5px; }

.bp3-list-unstyled{
  list-style:none;
  margin:0;
  padding:0; }
  .bp3-list-unstyled li{
    padding:0; }
.bp3-rtl{
  text-align:right; }

.bp3-dark{
  color:#f5f8fa; }

:focus{
  outline:rgba(19, 124, 189, 0.6) auto 2px;
  outline-offset:2px;
  -moz-outline-radius:6px; }

.bp3-focus-disabled :focus{
  outline:none !important; }
  .bp3-focus-disabled :focus ~ .bp3-control-indicator{
    outline:none !important; }

.bp3-alert{
  max-width:400px;
  padding:20px; }

.bp3-alert-body{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-alert-body .bp3-icon{
    font-size:40px;
    margin-right:20px;
    margin-top:0; }

.bp3-alert-contents{
  word-break:break-word; }

.bp3-alert-footer{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:reverse;
      -ms-flex-direction:row-reverse;
          flex-direction:row-reverse;
  margin-top:10px; }
  .bp3-alert-footer .bp3-button{
    margin-left:10px; }
.bp3-breadcrumbs{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  cursor:default;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:wrap;
      flex-wrap:wrap;
  height:30px;
  list-style:none;
  margin:0;
  padding:0; }
  .bp3-breadcrumbs > li{
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex; }
    .bp3-breadcrumbs > li::after{
      background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M10.71 7.29l-4-4a1.003 1.003 0 00-1.42 1.42L8.59 8 5.3 11.29c-.19.18-.3.43-.3.71a1.003 1.003 0 001.71.71l4-4c.18-.18.29-.43.29-.71 0-.28-.11-.53-.29-.71z' fill='%235C7080'/%3e%3c/svg%3e");
      content:"";
      display:block;
      height:16px;
      margin:0 5px;
      width:16px; }
    .bp3-breadcrumbs > li:last-of-type::after{
      display:none; }

.bp3-breadcrumb,
.bp3-breadcrumb-current,
.bp3-breadcrumbs-collapsed{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  font-size:16px; }

.bp3-breadcrumb,
.bp3-breadcrumbs-collapsed{
  color:#5c7080; }

.bp3-breadcrumb:hover{
  text-decoration:none; }

.bp3-breadcrumb.bp3-disabled{
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-breadcrumb .bp3-icon{
  margin-right:5px; }

.bp3-breadcrumb-current{
  color:inherit;
  font-weight:600; }
  .bp3-breadcrumb-current .bp3-input{
    font-size:inherit;
    font-weight:inherit;
    vertical-align:baseline; }

.bp3-breadcrumbs-collapsed{
  background:#ced9e0;
  border:none;
  border-radius:3px;
  cursor:pointer;
  margin-right:2px;
  padding:1px 5px;
  vertical-align:text-bottom; }
  .bp3-breadcrumbs-collapsed::before{
    background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cg fill='%235C7080'%3e%3ccircle cx='2' cy='8.03' r='2'/%3e%3ccircle cx='14' cy='8.03' r='2'/%3e%3ccircle cx='8' cy='8.03' r='2'/%3e%3c/g%3e%3c/svg%3e") center no-repeat;
    content:"";
    display:block;
    height:16px;
    width:16px; }
  .bp3-breadcrumbs-collapsed:hover{
    background:#bfccd6;
    color:#182026;
    text-decoration:none; }

.bp3-dark .bp3-breadcrumb,
.bp3-dark .bp3-breadcrumbs-collapsed{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumbs > li::after{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumb.bp3-disabled{
  color:rgba(167, 182, 194, 0.6); }

.bp3-dark .bp3-breadcrumb-current{
  color:#f5f8fa; }

.bp3-dark .bp3-breadcrumbs-collapsed{
  background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-breadcrumbs-collapsed:hover{
    background:rgba(16, 22, 26, 0.6);
    color:#f5f8fa; }
.bp3-button{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  font-size:14px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  padding:5px 10px;
  text-align:left;
  vertical-align:middle;
  min-height:30px;
  min-width:30px; }
  .bp3-button > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-button > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-button::before,
  .bp3-button > *{
    margin-right:7px; }
  .bp3-button:empty::before,
  .bp3-button > :last-child{
    margin-right:0; }
  .bp3-button:empty{
    padding:0 !important; }
  .bp3-button:disabled, .bp3-button.bp3-disabled{
    cursor:not-allowed; }
  .bp3-button.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button.bp3-align-right,
  .bp3-align-right .bp3-button{
    text-align:right; }
  .bp3-button.bp3-align-left,
  .bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-button:not([class*="bp3-intent-"]){
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    color:#182026; }
    .bp3-button:not([class*="bp3-intent-"]):hover{
      background-clip:padding-box;
      background-color:#ebf1f5;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
    .bp3-button:not([class*="bp3-intent-"]):active, .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      background-color:#d8e1e8;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      outline:none; }
      .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active:hover, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-button.bp3-intent-primary{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover, .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover{
      background-color:#106ba3;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      background-color:#0e5a8a;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-primary:disabled, .bp3-button.bp3-intent-primary.bp3-disabled{
      background-color:rgba(19, 124, 189, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-success{
    background-color:#0f9960;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-success:hover, .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-success:hover{
      background-color:#0d8050;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      background-color:#0a6640;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-success:disabled, .bp3-button.bp3-intent-success.bp3-disabled{
      background-color:rgba(15, 153, 96, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-warning{
    background-color:#d9822b;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover, .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover{
      background-color:#bf7326;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      background-color:#a66321;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-warning:disabled, .bp3-button.bp3-intent-warning.bp3-disabled{
      background-color:rgba(217, 130, 43, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-danger{
    background-color:#db3737;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover, .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover{
      background-color:#c23030;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      background-color:#a82a2a;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-danger:disabled, .bp3-button.bp3-intent-danger.bp3-disabled{
      background-color:rgba(219, 55, 55, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
    stroke:#ffffff; }
  .bp3-button.bp3-large,
  .bp3-large .bp3-button{
    min-height:40px;
    min-width:40px;
    font-size:16px;
    padding:5px 15px; }
    .bp3-button.bp3-large::before,
    .bp3-button.bp3-large > *,
    .bp3-large .bp3-button::before,
    .bp3-large .bp3-button > *{
      margin-right:10px; }
    .bp3-button.bp3-large:empty::before,
    .bp3-button.bp3-large > :last-child,
    .bp3-large .bp3-button:empty::before,
    .bp3-large .bp3-button > :last-child{
      margin-right:0; }
  .bp3-button.bp3-small,
  .bp3-small .bp3-button{
    min-height:24px;
    min-width:24px;
    padding:0 7px; }
  .bp3-button.bp3-loading{
    position:relative; }
    .bp3-button.bp3-loading[class*="bp3-icon-"]::before{
      visibility:hidden; }
    .bp3-button.bp3-loading .bp3-button-spinner{
      margin:0;
      position:absolute; }
    .bp3-button.bp3-loading > :not(.bp3-button-spinner){
      visibility:hidden; }
  .bp3-button[class*="bp3-icon-"]::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    color:#5c7080; }
  .bp3-button .bp3-icon, .bp3-button .bp3-icon-standard, .bp3-button .bp3-icon-large{
    color:#5c7080; }
    .bp3-button .bp3-icon.bp3-align-right, .bp3-button .bp3-icon-standard.bp3-align-right, .bp3-button .bp3-icon-large.bp3-align-right{
      margin-left:7px; }
  .bp3-button .bp3-icon:first-child:last-child,
  .bp3-button .bp3-spinner + .bp3-icon:last-child{
    margin:0 -7px; }
  .bp3-dark .bp3-button:not([class*="bp3-intent-"]){
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover, .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"])[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-large{
      color:#a7b6c2; }
  .bp3-dark .bp3-button[class*="bp3-intent-"]{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:hover{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:active, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-active{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:disabled, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-disabled{
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.3); }
    .bp3-dark .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
      stroke:#8a9ba8; }
  .bp3-button:disabled::before,
  .bp3-button:disabled .bp3-icon, .bp3-button:disabled .bp3-icon-standard, .bp3-button:disabled .bp3-icon-large, .bp3-button.bp3-disabled::before,
  .bp3-button.bp3-disabled .bp3-icon, .bp3-button.bp3-disabled .bp3-icon-standard, .bp3-button.bp3-disabled .bp3-icon-large, .bp3-button[class*="bp3-intent-"]::before,
  .bp3-button[class*="bp3-intent-"] .bp3-icon, .bp3-button[class*="bp3-intent-"] .bp3-icon-standard, .bp3-button[class*="bp3-intent-"] .bp3-icon-large{
    color:inherit !important; }
  .bp3-button.bp3-minimal{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-button.bp3-minimal:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button.bp3-minimal:active, .bp3-button.bp3-minimal.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button.bp3-minimal:disabled, .bp3-button.bp3-minimal:disabled:hover, .bp3-button.bp3-minimal.bp3-disabled, .bp3-button.bp3-minimal.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-minimal{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-minimal:hover, .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button.bp3-minimal:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-minimal:disabled, .bp3-dark .bp3-button.bp3-minimal:disabled:hover, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover, .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover, .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover, .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover, .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button.bp3-outlined{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    border:1px solid rgba(24, 32, 38, 0.2);
    -webkit-box-sizing:border-box;
            box-sizing:border-box; }
    .bp3-button.bp3-outlined:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button.bp3-outlined:active, .bp3-button.bp3-outlined.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-outlined{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-outlined:hover, .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button.bp3-outlined:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:hover, .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:hover, .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:hover, .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:hover, .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
    .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled:hover{
      border-color:rgba(92, 112, 128, 0.1); }
    .bp3-dark .bp3-button.bp3-outlined{
      border-color:rgba(255, 255, 255, 0.4); }
      .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
        border-color:rgba(255, 255, 255, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-primary{
      border-color:rgba(16, 107, 163, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
        border-color:rgba(16, 107, 163, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
        border-color:rgba(72, 175, 240, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
          border-color:rgba(72, 175, 240, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-success{
      border-color:rgba(13, 128, 80, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
        border-color:rgba(13, 128, 80, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
        border-color:rgba(61, 204, 145, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
          border-color:rgba(61, 204, 145, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-warning{
      border-color:rgba(191, 115, 38, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
        border-color:rgba(191, 115, 38, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
        border-color:rgba(255, 179, 102, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
          border-color:rgba(255, 179, 102, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-danger{
      border-color:rgba(194, 48, 48, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
        border-color:rgba(194, 48, 48, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
        border-color:rgba(255, 115, 115, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
          border-color:rgba(255, 115, 115, 0.2); }

a.bp3-button{
  text-align:center;
  text-decoration:none;
  -webkit-transition:none;
  transition:none; }
  a.bp3-button, a.bp3-button:hover, a.bp3-button:active{
    color:#182026; }
  a.bp3-button.bp3-disabled{
    color:rgba(92, 112, 128, 0.6); }

.bp3-button-text{
  -webkit-box-flex:0;
      -ms-flex:0 1 auto;
          flex:0 1 auto; }

.bp3-button.bp3-align-left .bp3-button-text, .bp3-button.bp3-align-right .bp3-button-text,
.bp3-button-group.bp3-align-left .bp3-button-text,
.bp3-button-group.bp3-align-right .bp3-button-text{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto; }
.bp3-button-group{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex; }
  .bp3-button-group .bp3-button{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    position:relative;
    z-index:4; }
    .bp3-button-group .bp3-button:focus{
      z-index:5; }
    .bp3-button-group .bp3-button:hover{
      z-index:6; }
    .bp3-button-group .bp3-button:active, .bp3-button-group .bp3-button.bp3-active{
      z-index:7; }
    .bp3-button-group .bp3-button:disabled, .bp3-button-group .bp3-button.bp3-disabled{
      z-index:3; }
    .bp3-button-group .bp3-button[class*="bp3-intent-"]{
      z-index:9; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:focus{
        z-index:10; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:hover{
        z-index:11; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:active, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-active{
        z-index:12; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:disabled, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-disabled{
        z-index:8; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:first-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:first-child){
    border-bottom-left-radius:0;
    border-top-left-radius:0; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    border-bottom-right-radius:0;
    border-top-right-radius:0;
    margin-right:-1px; }
  .bp3-button-group.bp3-minimal .bp3-button{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-button-group.bp3-minimal .bp3-button:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button-group.bp3-minimal .bp3-button{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
      color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
      color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button-group .bp3-popover-wrapper,
  .bp3-button-group .bp3-popover-target{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button-group .bp3-button.bp3-fill,
  .bp3-button-group.bp3-fill .bp3-button:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-vertical{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column;
    vertical-align:top; }
    .bp3-button-group.bp3-vertical.bp3-fill{
      height:100%;
      width:unset; }
    .bp3-button-group.bp3-vertical .bp3-button{
      margin-right:0 !important;
      width:100%; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:first-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:first-child{
      border-radius:3px 3px 0 0; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:last-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:last-child{
      border-radius:0 0 3px 3px; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:not(:last-child){
      margin-bottom:-1px; }
  .bp3-button-group.bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    margin-right:1px; }
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-button:not(:last-child){
    margin-bottom:1px; }
.bp3-callout{
  font-size:14px;
  line-height:1.5;
  background-color:rgba(138, 155, 168, 0.15);
  border-radius:3px;
  padding:10px 12px 9px;
  position:relative;
  width:100%; }
  .bp3-callout[class*="bp3-icon-"]{
    padding-left:40px; }
    .bp3-callout[class*="bp3-icon-"]::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      color:#5c7080;
      left:10px;
      position:absolute;
      top:10px; }
  .bp3-callout.bp3-callout-icon{
    padding-left:40px; }
    .bp3-callout.bp3-callout-icon > .bp3-icon:first-child{
      color:#5c7080;
      left:10px;
      position:absolute;
      top:10px; }
  .bp3-callout .bp3-heading{
    line-height:20px;
    margin-bottom:5px;
    margin-top:0; }
    .bp3-callout .bp3-heading:last-child{
      margin-bottom:0; }
  .bp3-dark .bp3-callout{
    background-color:rgba(138, 155, 168, 0.2); }
    .bp3-dark .bp3-callout[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
  .bp3-callout.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15); }
    .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-primary .bp3-heading{
      color:#106ba3; }
    .bp3-dark .bp3-callout.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-primary .bp3-heading{
        color:#48aff0; }
  .bp3-callout.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15); }
    .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-success .bp3-heading{
      color:#0d8050; }
    .bp3-dark .bp3-callout.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-success .bp3-heading{
        color:#3dcc91; }
  .bp3-callout.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15); }
    .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-warning .bp3-heading{
      color:#bf7326; }
    .bp3-dark .bp3-callout.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-warning .bp3-heading{
        color:#ffb366; }
  .bp3-callout.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15); }
    .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-danger .bp3-heading{
      color:#c23030; }
    .bp3-dark .bp3-callout.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-danger .bp3-heading{
        color:#ff7373; }
  .bp3-running-text .bp3-callout{
    margin:20px 0; }
.bp3-card{
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
  padding:20px;
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-card.bp3-dark,
  .bp3-dark .bp3-card{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-0{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }
  .bp3-elevation-0.bp3-dark,
  .bp3-dark .bp3-elevation-0{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-1{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-1.bp3-dark,
  .bp3-dark .bp3-elevation-1{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-elevation-2{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-2.bp3-dark,
  .bp3-dark .bp3-elevation-2{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4); }

.bp3-elevation-3{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-3.bp3-dark,
  .bp3-dark .bp3-elevation-3{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-elevation-4{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-4.bp3-dark,
  .bp3-dark .bp3-elevation-4{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:hover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  cursor:pointer; }
  .bp3-card.bp3-interactive:hover.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:hover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:active{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  opacity:0.9;
  -webkit-transition-duration:0;
          transition-duration:0; }
  .bp3-card.bp3-interactive:active.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:active{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-collapse{
  height:0;
  overflow-y:hidden;
  -webkit-transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-collapse .bp3-collapse-body{
    -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-collapse .bp3-collapse-body[aria-hidden="true"]{
      display:none; }

.bp3-context-menu .bp3-popover-target{
  display:block; }

.bp3-context-menu-popover-target{
  position:fixed; }

.bp3-divider{
  border-bottom:1px solid rgba(16, 22, 26, 0.15);
  border-right:1px solid rgba(16, 22, 26, 0.15);
  margin:5px; }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-dialog-container{
  opacity:1;
  -webkit-transform:scale(1);
          transform:scale(1);
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  min-height:100%;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none;
  width:100%; }
  .bp3-dialog-container.bp3-overlay-enter > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5); }
  .bp3-dialog-container.bp3-overlay-enter-active > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear-active > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-dialog-container.bp3-overlay-exit > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-dialog-container.bp3-overlay-exit-active > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }

.bp3-dialog{
  background:#ebf1f5;
  border-radius:6px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:30px 0;
  padding-bottom:20px;
  pointer-events:all;
  -webkit-user-select:text;
     -moz-user-select:text;
      -ms-user-select:text;
          user-select:text;
  width:500px; }
  .bp3-dialog:focus{
    outline:0; }
  .bp3-dialog.bp3-dark,
  .bp3-dark .bp3-dialog{
    background:#293742;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }

.bp3-dialog-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background:#ffffff;
  border-radius:6px 6px 0 0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  min-height:40px;
  padding-left:20px;
  padding-right:5px;
  z-index:30; }
  .bp3-dialog-header .bp3-icon-large,
  .bp3-dialog-header .bp3-icon{
    color:#5c7080;
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px; }
  .bp3-dialog-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:inherit;
    margin:0; }
    .bp3-dialog-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-dialog-header{
    background:#30404d;
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-dialog-header .bp3-icon-large,
    .bp3-dark .bp3-dialog-header .bp3-icon{
      color:#a7b6c2; }

.bp3-dialog-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  line-height:18px;
  margin:20px; }

.bp3-dialog-footer{
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  margin:0 20px; }

.bp3-dialog-footer-actions{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:end;
      -ms-flex-pack:end;
          justify-content:flex-end; }
  .bp3-dialog-footer-actions .bp3-button{
    margin-left:10px; }
.bp3-multistep-dialog-panels{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }

.bp3-multistep-dialog-left-panel{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:1;
      -ms-flex:1;
          flex:1;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column; }
  .bp3-dark .bp3-multistep-dialog-left-panel{
    background:#202b33; }

.bp3-multistep-dialog-right-panel{
  background-color:#f5f8fa;
  border-left:1px solid rgba(16, 22, 26, 0.15);
  border-radius:0 0 6px 0;
  -webkit-box-flex:3;
      -ms-flex:3;
          flex:3;
  min-width:0; }
  .bp3-dark .bp3-multistep-dialog-right-panel{
    background-color:#293742;
    border-left:1px solid rgba(16, 22, 26, 0.4); }

.bp3-multistep-dialog-footer{
  background-color:#ffffff;
  border-radius:0 0 6px 0;
  border-top:1px solid rgba(16, 22, 26, 0.15);
  padding:10px; }
  .bp3-dark .bp3-multistep-dialog-footer{
    background:#30404d;
    border-top:1px solid rgba(16, 22, 26, 0.4); }

.bp3-dialog-step-container{
  background-color:#f5f8fa;
  border-bottom:1px solid rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-dialog-step-container{
    background:#293742;
    border-bottom:1px solid rgba(16, 22, 26, 0.4); }
  .bp3-dialog-step-container.bp3-dialog-step-viewed{
    background-color:#ffffff; }
    .bp3-dark .bp3-dialog-step-container.bp3-dialog-step-viewed{
      background:#30404d; }

.bp3-dialog-step{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:#f5f8fa;
  border-radius:6px;
  cursor:not-allowed;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin:4px;
  padding:6px 14px; }
  .bp3-dark .bp3-dialog-step{
    background:#293742; }
  .bp3-dialog-step-viewed .bp3-dialog-step{
    background-color:#ffffff;
    cursor:pointer; }
    .bp3-dark .bp3-dialog-step-viewed .bp3-dialog-step{
      background:#30404d; }
  .bp3-dialog-step:hover{
    background-color:#f5f8fa; }
    .bp3-dark .bp3-dialog-step:hover{
      background:#293742; }

.bp3-dialog-step-icon{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:rgba(92, 112, 128, 0.6);
  border-radius:50%;
  color:#ffffff;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:25px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  width:25px; }
  .bp3-dark .bp3-dialog-step-icon{
    background-color:rgba(167, 182, 194, 0.6); }
  .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-icon{
    background-color:#2b95d6; }
  .bp3-dialog-step-viewed .bp3-dialog-step-icon{
    background-color:#8a9ba8; }

.bp3-dialog-step-title{
  color:rgba(92, 112, 128, 0.6);
  -webkit-box-flex:1;
      -ms-flex:1;
          flex:1;
  padding-left:10px; }
  .bp3-dark .bp3-dialog-step-title{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-title{
    color:#2b95d6; }
  .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
    color:#182026; }
    .bp3-dark .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
      color:#f5f8fa; }
.bp3-drawer{
  background:#ffffff;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0;
  padding:0; }
  .bp3-drawer:focus{
    outline:0; }
  .bp3-drawer.bp3-position-top{
    height:50%;
    left:0;
    right:0;
    top:0; }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter, .bp3-drawer.bp3-position-top.bp3-overlay-appear{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%); }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter-active, .bp3-drawer.bp3-position-top.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit-active{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-bottom{
    bottom:0;
    height:50%;
    left:0;
    right:0; }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter-active, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-left{
    bottom:0;
    left:0;
    top:0;
    width:50%; }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter, .bp3-drawer.bp3-position-left.bp3-overlay-appear{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%); }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter-active, .bp3-drawer.bp3-position-left.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit-active{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-right{
    bottom:0;
    right:0;
    top:0;
    width:50%; }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter, .bp3-drawer.bp3-position-right.bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter-active, .bp3-drawer.bp3-position-right.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right):not(.bp3-vertical){
    bottom:0;
    right:0;
    top:0;
    width:50%; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right).bp3-vertical{
    bottom:0;
    height:50%;
    left:0;
    right:0; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-dark,
  .bp3-dark .bp3-drawer{
    background:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }

.bp3-drawer-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border-radius:0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  min-height:40px;
  padding:5px;
  padding-left:20px;
  position:relative; }
  .bp3-drawer-header .bp3-icon-large,
  .bp3-drawer-header .bp3-icon{
    color:#5c7080;
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px; }
  .bp3-drawer-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:inherit;
    margin:0; }
    .bp3-drawer-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-drawer-header{
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-drawer-header .bp3-icon-large,
    .bp3-dark .bp3-drawer-header .bp3-icon{
      color:#a7b6c2; }

.bp3-drawer-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  line-height:18px;
  overflow:auto; }

.bp3-drawer-footer{
  -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  padding:10px 20px;
  position:relative; }
  .bp3-dark .bp3-drawer-footer{
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4); }
.bp3-editable-text{
  cursor:text;
  display:inline-block;
  max-width:100%;
  position:relative;
  vertical-align:top;
  white-space:nowrap; }
  .bp3-editable-text::before{
    bottom:-3px;
    left:-3px;
    position:absolute;
    right:-3px;
    top:-3px;
    border-radius:3px;
    content:"";
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-editable-text.bp3-editable-text-editing::before{
    background-color:#ffffff;
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#137cbd; }
  .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4); }
  .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#0f9960; }
  .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4); }
  .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#d9822b; }
  .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4); }
  .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#db3737; }
  .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4); }
  .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15); }
  .bp3-dark .bp3-editable-text.bp3-editable-text-editing::before{
    background-color:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#48aff0; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4);
            box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#3dcc91; }
  .bp3-dark .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4);
            box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#ffb366; }
  .bp3-dark .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4);
            box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#ff7373; }
  .bp3-dark .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4);
            box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-editable-text-input,
.bp3-editable-text-content{
  color:inherit;
  display:inherit;
  font:inherit;
  letter-spacing:inherit;
  max-width:inherit;
  min-width:inherit;
  position:relative;
  resize:none;
  text-transform:inherit;
  vertical-align:top; }

.bp3-editable-text-input{
  background:none;
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0;
  white-space:pre-wrap;
  width:100%; }
  .bp3-editable-text-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input:focus{
    outline:none; }
  .bp3-editable-text-input::-ms-clear{
    display:none; }

.bp3-editable-text-content{
  overflow:hidden;
  padding-right:2px;
  text-overflow:ellipsis;
  white-space:pre; }
  .bp3-editable-text-editing > .bp3-editable-text-content{
    left:0;
    position:absolute;
    visibility:hidden; }
  .bp3-editable-text-placeholder > .bp3-editable-text-content{
    color:rgba(92, 112, 128, 0.6); }
    .bp3-dark .bp3-editable-text-placeholder > .bp3-editable-text-content{
      color:rgba(167, 182, 194, 0.6); }

.bp3-editable-text.bp3-multiline{
  display:block; }
  .bp3-editable-text.bp3-multiline .bp3-editable-text-content{
    overflow:auto;
    white-space:pre-wrap;
    word-wrap:break-word; }
.bp3-divider{
  border-bottom:1px solid rgba(16, 22, 26, 0.15);
  border-right:1px solid rgba(16, 22, 26, 0.15);
  margin:5px; }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-control-group{
  -webkit-transform:translateZ(0);
          transform:translateZ(0);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:stretch;
      -ms-flex-align:stretch;
          align-items:stretch; }
  .bp3-control-group > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select,
  .bp3-control-group .bp3-input,
  .bp3-control-group .bp3-select{
    position:relative; }
  .bp3-control-group .bp3-input{
    border-radius:inherit;
    z-index:2; }
    .bp3-control-group .bp3-input:focus{
      border-radius:3px;
      z-index:14; }
    .bp3-control-group .bp3-input[class*="bp3-intent"]{
      z-index:13; }
      .bp3-control-group .bp3-input[class*="bp3-intent"]:focus{
        z-index:15; }
    .bp3-control-group .bp3-input[readonly], .bp3-control-group .bp3-input:disabled, .bp3-control-group .bp3-input.bp3-disabled{
      z-index:1; }
  .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input{
    z-index:13; }
    .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input:focus{
      z-index:15; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select select,
  .bp3-control-group .bp3-select select{
    -webkit-transform:translateZ(0);
            transform:translateZ(0);
    border-radius:inherit;
    z-index:4; }
    .bp3-control-group .bp3-button:focus,
    .bp3-control-group .bp3-html-select select:focus,
    .bp3-control-group .bp3-select select:focus{
      z-index:5; }
    .bp3-control-group .bp3-button:hover,
    .bp3-control-group .bp3-html-select select:hover,
    .bp3-control-group .bp3-select select:hover{
      z-index:6; }
    .bp3-control-group .bp3-button:active,
    .bp3-control-group .bp3-html-select select:active,
    .bp3-control-group .bp3-select select:active{
      z-index:7; }
    .bp3-control-group .bp3-button[readonly], .bp3-control-group .bp3-button:disabled, .bp3-control-group .bp3-button.bp3-disabled,
    .bp3-control-group .bp3-html-select select[readonly],
    .bp3-control-group .bp3-html-select select:disabled,
    .bp3-control-group .bp3-html-select select.bp3-disabled,
    .bp3-control-group .bp3-select select[readonly],
    .bp3-control-group .bp3-select select:disabled,
    .bp3-control-group .bp3-select select.bp3-disabled{
      z-index:3; }
    .bp3-control-group .bp3-button[class*="bp3-intent"],
    .bp3-control-group .bp3-html-select select[class*="bp3-intent"],
    .bp3-control-group .bp3-select select[class*="bp3-intent"]{
      z-index:9; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:focus{
        z-index:10; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:hover{
        z-index:11; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:active{
        z-index:12; }
      .bp3-control-group .bp3-button[class*="bp3-intent"][readonly], .bp3-control-group .bp3-button[class*="bp3-intent"]:disabled, .bp3-control-group .bp3-button[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"].bp3-disabled{
        z-index:8; }
  .bp3-control-group .bp3-input-group > .bp3-icon,
  .bp3-control-group .bp3-input-group > .bp3-button,
  .bp3-control-group .bp3-input-group > .bp3-input-left-container,
  .bp3-control-group .bp3-input-group > .bp3-input-action{
    z-index:16; }
  .bp3-control-group .bp3-select::after,
  .bp3-control-group .bp3-html-select::after,
  .bp3-control-group .bp3-select > .bp3-icon,
  .bp3-control-group .bp3-html-select > .bp3-icon{
    z-index:17; }
  .bp3-control-group .bp3-select:focus-within{
    z-index:5; }
  .bp3-control-group:not(.bp3-vertical) > *:not(.bp3-divider){
    margin-right:-1px; }
  .bp3-control-group:not(.bp3-vertical) > .bp3-divider:not(:first-child){
    margin-left:6px; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > *:not(.bp3-divider){
    margin-right:0; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > .bp3-button + .bp3-button{
    margin-left:1px; }
  .bp3-control-group .bp3-popover-wrapper,
  .bp3-control-group .bp3-popover-target{
    border-radius:inherit; }
  .bp3-control-group > :first-child{
    border-radius:3px 0 0 3px; }
  .bp3-control-group > :last-child{
    border-radius:0 3px 3px 0;
    margin-right:0; }
  .bp3-control-group > :only-child{
    border-radius:3px;
    margin-right:0; }
  .bp3-control-group .bp3-input-group .bp3-button{
    border-radius:3px; }
  .bp3-control-group .bp3-numeric-input:not(:first-child) .bp3-input-group{
    border-bottom-left-radius:0;
    border-top-left-radius:0; }
  .bp3-control-group.bp3-fill{
    width:100%; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-fill > *:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-vertical{
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-control-group.bp3-vertical > *{
      margin-top:-1px; }
    .bp3-control-group.bp3-vertical > :first-child{
      border-radius:3px 3px 0 0;
      margin-top:0; }
    .bp3-control-group.bp3-vertical > :last-child{
      border-radius:0 0 3px 3px; }
.bp3-control{
  cursor:pointer;
  display:block;
  margin-bottom:10px;
  position:relative;
  text-transform:none; }
  .bp3-control input:checked ~ .bp3-control-indicator{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
  .bp3-control:hover input:checked ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
  .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    background:#0e5a8a;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-control input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control:hover input:checked ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    background-color:#0e5a8a;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-control:not(.bp3-align-right){
    padding-left:26px; }
    .bp3-control:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-26px; }
  .bp3-control.bp3-align-right{
    padding-right:26px; }
    .bp3-control.bp3-align-right .bp3-control-indicator{
      margin-right:-26px; }
  .bp3-control.bp3-disabled{
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-control.bp3-inline{
    display:inline-block;
    margin-right:20px; }
  .bp3-control input{
    left:0;
    opacity:0;
    position:absolute;
    top:0;
    z-index:-1; }
  .bp3-control .bp3-control-indicator{
    background-clip:padding-box;
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    border:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    cursor:pointer;
    display:inline-block;
    font-size:16px;
    height:1em;
    margin-right:10px;
    margin-top:-3px;
    position:relative;
    -webkit-user-select:none;
       -moz-user-select:none;
        -ms-user-select:none;
            user-select:none;
    vertical-align:middle;
    width:1em; }
    .bp3-control .bp3-control-indicator::before{
      content:"";
      display:block;
      height:1em;
      width:1em; }
  .bp3-control:hover .bp3-control-indicator{
    background-color:#ebf1f5; }
  .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
    background:#d8e1e8;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    cursor:not-allowed; }
  .bp3-control input:focus ~ .bp3-control-indicator{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:2px;
    -moz-outline-radius:6px; }
  .bp3-control.bp3-align-right .bp3-control-indicator{
    float:right;
    margin-left:10px;
    margin-top:1px; }
  .bp3-control.bp3-large{
    font-size:16px; }
    .bp3-control.bp3-large:not(.bp3-align-right){
      padding-left:30px; }
      .bp3-control.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
        margin-left:-30px; }
    .bp3-control.bp3-large.bp3-align-right{
      padding-right:30px; }
      .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
        margin-right:-30px; }
    .bp3-control.bp3-large .bp3-control-indicator{
      font-size:20px; }
    .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-top:0; }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
  .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
  .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    background:#0e5a8a;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    background-color:#0e5a8a;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-control.bp3-checkbox .bp3-control-indicator{
    border-radius:3px; }
  .bp3-control.bp3-checkbox input:checked ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 00-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0012 5z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-radio .bp3-control-indicator{
    border-radius:50%; }
  .bp3-control.bp3-radio input:checked ~ .bp3-control-indicator::before{
    background-image:radial-gradient(#ffffff, #ffffff 28%, transparent 32%); }
  .bp3-control.bp3-radio input:checked:disabled ~ .bp3-control-indicator::before{
    opacity:0.5; }
  .bp3-control.bp3-radio input:focus ~ .bp3-control-indicator{
    -moz-outline-radius:16px; }
  .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(167, 182, 194, 0.5); }
  .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(115, 134, 148, 0.5); }
  .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(92, 112, 128, 0.5); }
  .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5); }
    .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5); }
    .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch:not(.bp3-align-right){
    padding-left:38px; }
    .bp3-control.bp3-switch:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-38px; }
  .bp3-control.bp3-switch.bp3-align-right{
    padding-right:38px; }
    .bp3-control.bp3-switch.bp3-align-right .bp3-control-indicator{
      margin-right:-38px; }
  .bp3-control.bp3-switch .bp3-control-indicator{
    border:none;
    border-radius:1.75em;
    -webkit-box-shadow:none !important;
            box-shadow:none !important;
    min-width:1.75em;
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    width:auto; }
    .bp3-control.bp3-switch .bp3-control-indicator::before{
      background:#ffffff;
      border-radius:50%;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
      height:calc(1em - 4px);
      left:0;
      margin:2px;
      position:absolute;
      -webkit-transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      width:calc(1em - 4px); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    left:calc(100% - 1em); }
  .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right){
    padding-left:45px; }
    .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-45px; }
  .bp3-control.bp3-switch.bp3-large.bp3-align-right{
    padding-right:45px; }
    .bp3-control.bp3-switch.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-right:-45px; }
  .bp3-dark .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.7); }
  .bp3-dark .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.9); }
  .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(57, 75, 89, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-dark .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-dark .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch .bp3-control-indicator::before{
    background:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-control.bp3-switch .bp3-switch-inner-text{
    font-size:0.7em;
    text-align:center; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:first-child{
    line-height:0;
    margin-left:0.5em;
    margin-right:1.2em;
    visibility:hidden; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:last-child{
    line-height:1em;
    margin-left:1.2em;
    margin-right:0.5em;
    visibility:visible; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:first-child{
    line-height:1em;
    visibility:visible; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:last-child{
    line-height:0;
    visibility:hidden; }
  .bp3-dark .bp3-control{
    color:#f5f8fa; }
    .bp3-dark .bp3-control.bp3-disabled{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-control .bp3-control-indicator{
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-control:hover .bp3-control-indicator{
      background-color:#30404d; }
    .bp3-dark .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
      background:#202b33;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-control input:disabled ~ .bp3-control-indicator{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      cursor:not-allowed; }
    .bp3-dark .bp3-control.bp3-checkbox input:disabled:checked ~ .bp3-control-indicator, .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
      color:rgba(167, 182, 194, 0.6); }
.bp3-file-input{
  cursor:pointer;
  display:inline-block;
  height:30px;
  position:relative; }
  .bp3-file-input input{
    margin:0;
    min-width:200px;
    opacity:0; }
    .bp3-file-input input:disabled + .bp3-file-upload-input,
    .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
      background:rgba(206, 217, 224, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      resize:none; }
      .bp3-file-input input:disabled + .bp3-file-upload-input::after,
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
        background-color:rgba(206, 217, 224, 0.5);
        background-image:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(92, 112, 128, 0.6);
        cursor:not-allowed;
        outline:none; }
        .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active:hover,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active:hover{
          background:rgba(206, 217, 224, 0.7); }
      .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input, .bp3-dark
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
        background:rgba(57, 75, 89, 0.5);
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after, .bp3-dark
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
          background-color:rgba(57, 75, 89, 0.5);
          background-image:none;
          -webkit-box-shadow:none;
                  box-shadow:none;
          color:rgba(167, 182, 194, 0.6); }
          .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-dark
          .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active{
            background:rgba(57, 75, 89, 0.7); }
  .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#182026; }
  .bp3-dark .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#f5f8fa; }
  .bp3-file-input.bp3-fill{
    width:100%; }
  .bp3-file-input.bp3-large,
  .bp3-large .bp3-file-input{
    height:40px; }
  .bp3-file-input .bp3-file-upload-input-custom-text::after{
    content:attr(bp3-button-text); }

.bp3-file-upload-input{
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  background:#ffffff;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#182026;
  font-size:14px;
  font-weight:400;
  height:30px;
  line-height:30px;
  outline:none;
  padding:0 10px;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  vertical-align:middle;
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  color:rgba(92, 112, 128, 0.6);
  left:0;
  padding-right:80px;
  position:absolute;
  right:0;
  top:0;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-file-upload-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input:focus, .bp3-file-upload-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-file-upload-input[type="search"], .bp3-file-upload-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-file-upload-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-file-upload-input:disabled, .bp3-file-upload-input.bp3-disabled{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    resize:none; }
  .bp3-file-upload-input::after{
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    color:#182026;
    min-height:24px;
    min-width:24px;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    border-radius:3px;
    content:"Browse";
    line-height:24px;
    margin:3px;
    position:absolute;
    right:0;
    text-align:center;
    top:0;
    width:70px; }
    .bp3-file-upload-input::after:hover{
      background-clip:padding-box;
      background-color:#ebf1f5;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
    .bp3-file-upload-input::after:active, .bp3-file-upload-input::after.bp3-active{
      background-color:#d8e1e8;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-file-upload-input::after:disabled, .bp3-file-upload-input::after.bp3-disabled{
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      outline:none; }
      .bp3-file-upload-input::after:disabled.bp3-active, .bp3-file-upload-input::after:disabled.bp3-active:hover, .bp3-file-upload-input::after.bp3-disabled.bp3-active, .bp3-file-upload-input::after.bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-file-upload-input:hover::after{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-file-upload-input:active::after{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-large .bp3-file-upload-input{
    font-size:16px;
    height:40px;
    line-height:40px;
    padding-right:95px; }
    .bp3-large .bp3-file-upload-input[type="search"], .bp3-large .bp3-file-upload-input.bp3-round{
      padding:0 15px; }
    .bp3-large .bp3-file-upload-input::after{
      min-height:30px;
      min-width:30px;
      line-height:30px;
      margin:5px;
      width:85px; }
  .bp3-dark .bp3-file-upload-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:disabled, .bp3-dark .bp3-file-upload-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::after{
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover, .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover{
        background-color:#30404d;
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        background-color:#202b33;
        background-image:none;
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
      .bp3-dark .bp3-file-upload-input::after:disabled, .bp3-dark .bp3-file-upload-input::after.bp3-disabled{
        background-color:rgba(57, 75, 89, 0.5);
        background-image:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-upload-input::after:disabled.bp3-active, .bp3-dark .bp3-file-upload-input::after.bp3-disabled.bp3-active{
          background:rgba(57, 75, 89, 0.7); }
      .bp3-dark .bp3-file-upload-input::after .bp3-button-spinner .bp3-spinner-head{
        background:rgba(16, 22, 26, 0.5);
        stroke:#8a9ba8; }
    .bp3-dark .bp3-file-upload-input:hover::after{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:active::after{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
.bp3-file-upload-input::after{
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
.bp3-form-group{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0 0 15px; }
  .bp3-form-group label.bp3-label{
    margin-bottom:5px; }
  .bp3-form-group .bp3-control{
    margin-top:7px; }
  .bp3-form-group .bp3-form-helper-text{
    color:#5c7080;
    font-size:12px;
    margin-top:5px; }
  .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#106ba3; }
  .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#0d8050; }
  .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#bf7326; }
  .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#c23030; }
  .bp3-form-group.bp3-inline{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row; }
    .bp3-form-group.bp3-inline.bp3-large label.bp3-label{
      line-height:40px;
      margin:0 10px 0 0; }
    .bp3-form-group.bp3-inline label.bp3-label{
      line-height:30px;
      margin:0 10px 0 0; }
  .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-dark .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#48aff0; }
  .bp3-dark .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#3dcc91; }
  .bp3-dark .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#ffb366; }
  .bp3-dark .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#ff7373; }
  .bp3-dark .bp3-form-group .bp3-form-helper-text{
    color:#a7b6c2; }
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(167, 182, 194, 0.6) !important; }
.bp3-input-group{
  display:block;
  position:relative; }
  .bp3-input-group .bp3-input{
    position:relative;
    width:100%; }
    .bp3-input-group .bp3-input:not(:first-child){
      padding-left:30px; }
    .bp3-input-group .bp3-input:not(:last-child){
      padding-right:30px; }
  .bp3-input-group .bp3-input-action,
  .bp3-input-group > .bp3-input-left-container,
  .bp3-input-group > .bp3-button,
  .bp3-input-group > .bp3-icon{
    position:absolute;
    top:0; }
    .bp3-input-group .bp3-input-action:first-child,
    .bp3-input-group > .bp3-input-left-container:first-child,
    .bp3-input-group > .bp3-button:first-child,
    .bp3-input-group > .bp3-icon:first-child{
      left:0; }
    .bp3-input-group .bp3-input-action:last-child,
    .bp3-input-group > .bp3-input-left-container:last-child,
    .bp3-input-group > .bp3-button:last-child,
    .bp3-input-group > .bp3-icon:last-child{
      right:0; }
  .bp3-input-group .bp3-button{
    min-height:24px;
    min-width:24px;
    margin:3px;
    padding:0 7px; }
    .bp3-input-group .bp3-button:empty{
      padding:0; }
  .bp3-input-group > .bp3-input-left-container,
  .bp3-input-group > .bp3-icon{
    z-index:1; }
  .bp3-input-group > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group > .bp3-icon{
    color:#5c7080; }
    .bp3-input-group > .bp3-input-left-container > .bp3-icon:empty,
    .bp3-input-group > .bp3-icon:empty{
      font-family:"Icons16", sans-serif;
      font-size:16px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased; }
  .bp3-input-group > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group > .bp3-icon,
  .bp3-input-group .bp3-input-action > .bp3-spinner{
    margin:7px; }
  .bp3-input-group .bp3-tag{
    margin:5px; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus),
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
    color:#5c7080; }
    .bp3-dark .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus), .bp3-dark
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
      color:#a7b6c2; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large{
      color:#5c7080; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled,
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled{
    color:rgba(92, 112, 128, 0.6) !important; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-large{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-input-group.bp3-disabled{
    cursor:not-allowed; }
    .bp3-input-group.bp3-disabled .bp3-icon{
      color:rgba(92, 112, 128, 0.6); }
  .bp3-input-group.bp3-large .bp3-button{
    min-height:30px;
    min-width:30px;
    margin:5px; }
  .bp3-input-group.bp3-large > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group.bp3-large > .bp3-icon,
  .bp3-input-group.bp3-large .bp3-input-action > .bp3-spinner{
    margin:12px; }
  .bp3-input-group.bp3-large .bp3-input{
    font-size:16px;
    height:40px;
    line-height:40px; }
    .bp3-input-group.bp3-large .bp3-input[type="search"], .bp3-input-group.bp3-large .bp3-input.bp3-round{
      padding:0 15px; }
    .bp3-input-group.bp3-large .bp3-input:not(:first-child){
      padding-left:40px; }
    .bp3-input-group.bp3-large .bp3-input:not(:last-child){
      padding-right:40px; }
  .bp3-input-group.bp3-small .bp3-button{
    min-height:20px;
    min-width:20px;
    margin:2px; }
  .bp3-input-group.bp3-small .bp3-tag{
    min-height:20px;
    min-width:20px;
    margin:2px; }
  .bp3-input-group.bp3-small > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group.bp3-small > .bp3-icon,
  .bp3-input-group.bp3-small .bp3-input-action > .bp3-spinner{
    margin:4px; }
  .bp3-input-group.bp3-small .bp3-input{
    font-size:12px;
    height:24px;
    line-height:24px;
    padding-left:8px;
    padding-right:8px; }
    .bp3-input-group.bp3-small .bp3-input[type="search"], .bp3-input-group.bp3-small .bp3-input.bp3-round{
      padding:0 12px; }
    .bp3-input-group.bp3-small .bp3-input:not(:first-child){
      padding-left:24px; }
    .bp3-input-group.bp3-small .bp3-input:not(:last-child){
      padding-right:24px; }
  .bp3-input-group.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-input-group.bp3-round .bp3-button,
  .bp3-input-group.bp3-round .bp3-input,
  .bp3-input-group.bp3-round .bp3-tag{
    border-radius:30px; }
  .bp3-dark .bp3-input-group .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-input-group.bp3-disabled .bp3-icon{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-input-group.bp3-intent-primary .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input-group.bp3-intent-primary .bp3-input:disabled, .bp3-input-group.bp3-intent-primary .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-primary > .bp3-icon{
    color:#106ba3; }
    .bp3-dark .bp3-input-group.bp3-intent-primary > .bp3-icon{
      color:#48aff0; }
  .bp3-input-group.bp3-intent-success .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input-group.bp3-intent-success .bp3-input:disabled, .bp3-input-group.bp3-intent-success .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-success > .bp3-icon{
    color:#0d8050; }
    .bp3-dark .bp3-input-group.bp3-intent-success > .bp3-icon{
      color:#3dcc91; }
  .bp3-input-group.bp3-intent-warning .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input-group.bp3-intent-warning .bp3-input:disabled, .bp3-input-group.bp3-intent-warning .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-warning > .bp3-icon{
    color:#bf7326; }
    .bp3-dark .bp3-input-group.bp3-intent-warning > .bp3-icon{
      color:#ffb366; }
  .bp3-input-group.bp3-intent-danger .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input-group.bp3-intent-danger .bp3-input:disabled, .bp3-input-group.bp3-intent-danger .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-danger > .bp3-icon{
    color:#c23030; }
    .bp3-dark .bp3-input-group.bp3-intent-danger > .bp3-icon{
      color:#ff7373; }
.bp3-input{
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  background:#ffffff;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#182026;
  font-size:14px;
  font-weight:400;
  height:30px;
  line-height:30px;
  outline:none;
  padding:0 10px;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  vertical-align:middle; }
  .bp3-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input:focus, .bp3-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-input[type="search"], .bp3-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-input:disabled, .bp3-input.bp3-disabled{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    resize:none; }
  .bp3-input.bp3-large{
    font-size:16px;
    height:40px;
    line-height:40px; }
    .bp3-input.bp3-large[type="search"], .bp3-input.bp3-large.bp3-round{
      padding:0 15px; }
  .bp3-input.bp3-small{
    font-size:12px;
    height:24px;
    line-height:24px;
    padding-left:8px;
    padding-right:8px; }
    .bp3-input.bp3-small[type="search"], .bp3-input.bp3-small.bp3-round{
      padding:0 12px; }
  .bp3-input.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-dark .bp3-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input:disabled, .bp3-dark .bp3-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-input.bp3-intent-primary{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input.bp3-intent-primary:disabled, .bp3-input.bp3-intent-primary.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary:focus{
        -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #137cbd;
                box-shadow:inset 0 0 0 1px #137cbd; }
      .bp3-dark .bp3-input.bp3-intent-primary:disabled, .bp3-dark .bp3-input.bp3-intent-primary.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-success{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input.bp3-intent-success:disabled, .bp3-input.bp3-intent-success.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-success{
      -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success:focus{
        -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #0f9960;
                box-shadow:inset 0 0 0 1px #0f9960; }
      .bp3-dark .bp3-input.bp3-intent-success:disabled, .bp3-dark .bp3-input.bp3-intent-success.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-warning{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input.bp3-intent-warning:disabled, .bp3-input.bp3-intent-warning.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning:focus{
        -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #d9822b;
                box-shadow:inset 0 0 0 1px #d9822b; }
      .bp3-dark .bp3-input.bp3-intent-warning:disabled, .bp3-dark .bp3-input.bp3-intent-warning.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-danger{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input.bp3-intent-danger:disabled, .bp3-input.bp3-intent-danger.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger:focus{
        -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #db3737;
                box-shadow:inset 0 0 0 1px #db3737; }
      .bp3-dark .bp3-input.bp3-intent-danger:disabled, .bp3-dark .bp3-input.bp3-intent-danger.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input::-ms-clear{
    display:none; }
textarea.bp3-input{
  max-width:100%;
  padding:10px; }
  textarea.bp3-input, textarea.bp3-input.bp3-large, textarea.bp3-input.bp3-small{
    height:auto;
    line-height:inherit; }
  textarea.bp3-input.bp3-small{
    padding:8px; }
  .bp3-dark textarea.bp3-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark textarea.bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input:disabled, .bp3-dark textarea.bp3-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
label.bp3-label{
  display:block;
  margin-bottom:15px;
  margin-top:0; }
  label.bp3-label .bp3-html-select,
  label.bp3-label .bp3-input,
  label.bp3-label .bp3-select,
  label.bp3-label .bp3-slider,
  label.bp3-label .bp3-popover-wrapper{
    display:block;
    margin-top:5px;
    text-transform:none; }
  label.bp3-label .bp3-button-group{
    margin-top:5px; }
  label.bp3-label .bp3-select select,
  label.bp3-label .bp3-html-select select{
    font-weight:400;
    vertical-align:top;
    width:100%; }
  label.bp3-label.bp3-disabled,
  label.bp3-label.bp3-disabled .bp3-text-muted{
    color:rgba(92, 112, 128, 0.6); }
  label.bp3-label.bp3-inline{
    line-height:30px; }
    label.bp3-label.bp3-inline .bp3-html-select,
    label.bp3-label.bp3-inline .bp3-input,
    label.bp3-label.bp3-inline .bp3-input-group,
    label.bp3-label.bp3-inline .bp3-select,
    label.bp3-label.bp3-inline .bp3-popover-wrapper{
      display:inline-block;
      margin:0 0 0 5px;
      vertical-align:top; }
    label.bp3-label.bp3-inline .bp3-button-group{
      margin:0 0 0 5px; }
    label.bp3-label.bp3-inline .bp3-input-group .bp3-input{
      margin-left:0; }
    label.bp3-label.bp3-inline.bp3-large{
      line-height:40px; }
  label.bp3-label:not(.bp3-inline) .bp3-popover-target{
    display:block; }
  .bp3-dark label.bp3-label{
    color:#f5f8fa; }
    .bp3-dark label.bp3-label.bp3-disabled,
    .bp3-dark label.bp3-label.bp3-disabled .bp3-text-muted{
      color:rgba(167, 182, 194, 0.6); }
.bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button{
  -webkit-box-flex:1;
      -ms-flex:1 1 14px;
          flex:1 1 14px;
  min-height:0;
  padding:0;
  width:30px; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:first-child{
    border-radius:0 3px 0 0; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:last-child{
    border-radius:0 0 3px 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:first-child{
  border-radius:3px 0 0 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:last-child{
  border-radius:0 0 0 3px; }

.bp3-numeric-input.bp3-large .bp3-button-group.bp3-vertical > .bp3-button{
  width:40px; }

form{
  display:block; }
.bp3-html-select select,
.bp3-select select{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  font-size:14px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  padding:5px 10px;
  text-align:left;
  vertical-align:middle;
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  color:#182026;
  -moz-appearance:none;
  -webkit-appearance:none;
  border-radius:3px;
  height:30px;
  padding:0 25px 0 10px;
  width:100%; }
  .bp3-html-select select > *, .bp3-select select > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-html-select select > .bp3-fill, .bp3-select select > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-html-select select::before,
  .bp3-select select::before, .bp3-html-select select > *, .bp3-select select > *{
    margin-right:7px; }
  .bp3-html-select select:empty::before,
  .bp3-select select:empty::before,
  .bp3-html-select select > :last-child,
  .bp3-select select > :last-child{
    margin-right:0; }
  .bp3-html-select select:hover,
  .bp3-select select:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-html-select select:active,
  .bp3-select select:active, .bp3-html-select select.bp3-active,
  .bp3-select select.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-html-select select:disabled,
  .bp3-select select:disabled, .bp3-html-select select.bp3-disabled,
  .bp3-select select.bp3-disabled{
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    outline:none; }
    .bp3-html-select select:disabled.bp3-active,
    .bp3-select select:disabled.bp3-active, .bp3-html-select select:disabled.bp3-active:hover,
    .bp3-select select:disabled.bp3-active:hover, .bp3-html-select select.bp3-disabled.bp3-active,
    .bp3-select select.bp3-disabled.bp3-active, .bp3-html-select select.bp3-disabled.bp3-active:hover,
    .bp3-select select.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }

.bp3-html-select.bp3-minimal select,
.bp3-select.bp3-minimal select{
  background:none;
  -webkit-box-shadow:none;
          box-shadow:none; }
  .bp3-html-select.bp3-minimal select:hover,
  .bp3-select.bp3-minimal select:hover{
    background:rgba(167, 182, 194, 0.3);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:#182026;
    text-decoration:none; }
  .bp3-html-select.bp3-minimal select:active,
  .bp3-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal select.bp3-active,
  .bp3-select.bp3-minimal select.bp3-active{
    background:rgba(115, 134, 148, 0.3);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:#182026; }
  .bp3-html-select.bp3-minimal select:disabled,
  .bp3-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal select:disabled:hover,
  .bp3-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal select.bp3-disabled,
  .bp3-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal select.bp3-disabled:hover,
  .bp3-select.bp3-minimal select.bp3-disabled:hover{
    background:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
    .bp3-html-select.bp3-minimal select:disabled.bp3-active,
    .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active{
      background:rgba(115, 134, 148, 0.3); }
  .bp3-dark .bp3-html-select.bp3-minimal select, .bp3-html-select.bp3-minimal .bp3-dark select,
  .bp3-dark .bp3-select.bp3-minimal select, .bp3-select.bp3-minimal .bp3-dark select{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:inherit; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover, .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover{
      background:rgba(138, 155, 168, 0.15); }
    .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:rgba(138, 155, 168, 0.3);
      color:#f5f8fa; }
    .bp3-dark .bp3-html-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal .bp3-dark select:disabled,
    .bp3-dark .bp3-select.bp3-minimal select:disabled, .bp3-select.bp3-minimal .bp3-dark select:disabled, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select:disabled:hover, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover{
      background:none;
      color:rgba(167, 182, 194, 0.6);
      cursor:not-allowed; }
      .bp3-dark .bp3-html-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active{
        background:rgba(138, 155, 168, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-primary,
  .bp3-select.bp3-minimal select.bp3-intent-primary{
    color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover{
      background:rgba(19, 124, 189, 0.15);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:rgba(19, 124, 189, 0.3);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled{
      background:none;
      color:rgba(16, 107, 163, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active{
        background:rgba(19, 124, 189, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
      stroke:#106ba3; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary{
      color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.2);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(72, 175, 240, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-success,
  .bp3-select.bp3-minimal select.bp3-intent-success{
    color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover{
      background:rgba(15, 153, 96, 0.15);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:rgba(15, 153, 96, 0.3);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled{
      background:none;
      color:rgba(13, 128, 80, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active{
        background:rgba(15, 153, 96, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
      stroke:#0d8050; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success{
      color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.2);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(61, 204, 145, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-warning,
  .bp3-select.bp3-minimal select.bp3-intent-warning{
    color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover{
      background:rgba(217, 130, 43, 0.15);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:rgba(217, 130, 43, 0.3);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled{
      background:none;
      color:rgba(191, 115, 38, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active{
        background:rgba(217, 130, 43, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
      stroke:#bf7326; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning{
      color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.2);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(255, 179, 102, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-danger,
  .bp3-select.bp3-minimal select.bp3-intent-danger{
    color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover{
      background:rgba(219, 55, 55, 0.15);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:rgba(219, 55, 55, 0.3);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled{
      background:none;
      color:rgba(194, 48, 48, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active{
        background:rgba(219, 55, 55, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
      stroke:#c23030; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger{
      color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.2);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(255, 115, 115, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }

.bp3-html-select.bp3-large select,
.bp3-select.bp3-large select{
  font-size:16px;
  height:40px;
  padding-right:35px; }

.bp3-dark .bp3-html-select select, .bp3-dark .bp3-select select{
  background-color:#394b59;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
  color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover, .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    background-color:#202b33;
    background-image:none;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-html-select select:disabled, .bp3-dark .bp3-select select:disabled, .bp3-dark .bp3-html-select select.bp3-disabled, .bp3-dark .bp3-select select.bp3-disabled{
    background-color:rgba(57, 75, 89, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-html-select select:disabled.bp3-active, .bp3-dark .bp3-select select:disabled.bp3-active, .bp3-dark .bp3-html-select select.bp3-disabled.bp3-active, .bp3-dark .bp3-select select.bp3-disabled.bp3-active{
      background:rgba(57, 75, 89, 0.7); }
  .bp3-dark .bp3-html-select select .bp3-button-spinner .bp3-spinner-head, .bp3-dark .bp3-select select .bp3-button-spinner .bp3-spinner-head{
    background:rgba(16, 22, 26, 0.5);
    stroke:#8a9ba8; }

.bp3-html-select select:disabled,
.bp3-select select:disabled{
  background-color:rgba(206, 217, 224, 0.5);
  -webkit-box-shadow:none;
          box-shadow:none;
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-html-select .bp3-icon,
.bp3-select .bp3-icon, .bp3-select::after{
  color:#5c7080;
  pointer-events:none;
  position:absolute;
  right:7px;
  top:7px; }
  .bp3-html-select .bp3-disabled.bp3-icon,
  .bp3-select .bp3-disabled.bp3-icon, .bp3-disabled.bp3-select::after{
    color:rgba(92, 112, 128, 0.6); }
.bp3-html-select,
.bp3-select{
  display:inline-block;
  letter-spacing:normal;
  position:relative;
  vertical-align:middle; }
  .bp3-html-select select::-ms-expand,
  .bp3-select select::-ms-expand{
    display:none; }
  .bp3-html-select .bp3-icon,
  .bp3-select .bp3-icon{
    color:#5c7080; }
    .bp3-html-select .bp3-icon:hover,
    .bp3-select .bp3-icon:hover{
      color:#182026; }
    .bp3-dark .bp3-html-select .bp3-icon, .bp3-dark
    .bp3-select .bp3-icon{
      color:#a7b6c2; }
      .bp3-dark .bp3-html-select .bp3-icon:hover, .bp3-dark
      .bp3-select .bp3-icon:hover{
        color:#f5f8fa; }
  .bp3-html-select.bp3-large::after,
  .bp3-html-select.bp3-large .bp3-icon,
  .bp3-select.bp3-large::after,
  .bp3-select.bp3-large .bp3-icon{
    right:12px;
    top:12px; }
  .bp3-html-select.bp3-fill,
  .bp3-html-select.bp3-fill select,
  .bp3-select.bp3-fill,
  .bp3-select.bp3-fill select{
    width:100%; }
  .bp3-dark .bp3-html-select option, .bp3-dark
  .bp3-select option{
    background-color:#30404d;
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select option:disabled, .bp3-dark
  .bp3-select option:disabled{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-html-select::after, .bp3-dark
  .bp3-select::after{
    color:#a7b6c2; }

.bp3-select::after{
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  content:""; }
.bp3-running-text table, table.bp3-html-table{
  border-spacing:0;
  font-size:14px; }
  .bp3-running-text table th, table.bp3-html-table th,
  .bp3-running-text table td,
  table.bp3-html-table td{
    padding:11px;
    text-align:left;
    vertical-align:top; }
  .bp3-running-text table th, table.bp3-html-table th{
    color:#182026;
    font-weight:600; }
  
  .bp3-running-text table td,
  table.bp3-html-table td{
    color:#182026; }
  .bp3-running-text table tbody tr:first-child th, table.bp3-html-table tbody tr:first-child th,
  .bp3-running-text table tbody tr:first-child td,
  table.bp3-html-table tbody tr:first-child td,
  .bp3-running-text table tfoot tr:first-child th,
  table.bp3-html-table tfoot tr:first-child th,
  .bp3-running-text table tfoot tr:first-child td,
  table.bp3-html-table tfoot tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-running-text table th, .bp3-running-text .bp3-dark table th, .bp3-dark table.bp3-html-table th{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table td, .bp3-running-text .bp3-dark table td, .bp3-dark table.bp3-html-table td{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table tbody tr:first-child th, .bp3-running-text .bp3-dark table tbody tr:first-child th, .bp3-dark table.bp3-html-table tbody tr:first-child th,
  .bp3-dark .bp3-running-text table tbody tr:first-child td,
  .bp3-running-text .bp3-dark table tbody tr:first-child td,
  .bp3-dark table.bp3-html-table tbody tr:first-child td,
  .bp3-dark .bp3-running-text table tfoot tr:first-child th,
  .bp3-running-text .bp3-dark table tfoot tr:first-child th,
  .bp3-dark table.bp3-html-table tfoot tr:first-child th,
  .bp3-dark .bp3-running-text table tfoot tr:first-child td,
  .bp3-running-text .bp3-dark table tfoot tr:first-child td,
  .bp3-dark table.bp3-html-table tfoot tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }

table.bp3-html-table.bp3-html-table-condensed th,
table.bp3-html-table.bp3-html-table-condensed td, table.bp3-html-table.bp3-small th,
table.bp3-html-table.bp3-small td{
  padding-bottom:6px;
  padding-top:6px; }

table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
  background:rgba(191, 204, 214, 0.15); }

table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
  -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered tbody tr td,
table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
  -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
  table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
    -webkit-box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
  -webkit-box-shadow:none;
          box-shadow:none; }
  table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-interactive tbody tr:hover td{
  background-color:rgba(191, 204, 214, 0.3);
  cursor:pointer; }

table.bp3-html-table.bp3-interactive tbody tr:active td{
  background-color:rgba(191, 204, 214, 0.4); }

.bp3-dark table.bp3-html-table{ }
  .bp3-dark table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
    background:rgba(92, 112, 128, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td,
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
      -webkit-box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15);
              box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
    -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:first-child{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:hover td{
    background-color:rgba(92, 112, 128, 0.3);
    cursor:pointer; }
  .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:active td{
    background-color:rgba(92, 112, 128, 0.4); }

.bp3-key-combo{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center; }
  .bp3-key-combo > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-key-combo > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-key-combo::before,
  .bp3-key-combo > *{
    margin-right:5px; }
  .bp3-key-combo:empty::before,
  .bp3-key-combo > :last-child{
    margin-right:0; }

.bp3-hotkey-dialog{
  padding-bottom:0;
  top:40px; }
  .bp3-hotkey-dialog .bp3-dialog-body{
    margin:0;
    padding:0; }
  .bp3-hotkey-dialog .bp3-hotkey-label{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1; }

.bp3-hotkey-column{
  margin:auto;
  max-height:80vh;
  overflow-y:auto;
  padding:30px; }
  .bp3-hotkey-column .bp3-heading{
    margin-bottom:20px; }
    .bp3-hotkey-column .bp3-heading:not(:first-child){
      margin-top:40px; }

.bp3-hotkey{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:justify;
      -ms-flex-pack:justify;
          justify-content:space-between;
  margin-left:0;
  margin-right:0; }
  .bp3-hotkey:not(:last-child){
    margin-bottom:10px; }
.bp3-icon{
  display:inline-block;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  vertical-align:text-bottom; }
  .bp3-icon:not(:empty)::before{
    content:"" !important;
    content:unset !important; }
  .bp3-icon > svg{
    display:block; }
    .bp3-icon > svg:not([fill]){
      fill:currentColor; }

.bp3-icon.bp3-intent-primary, .bp3-icon-standard.bp3-intent-primary, .bp3-icon-large.bp3-intent-primary{
  color:#106ba3; }
  .bp3-dark .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-icon-large.bp3-intent-primary{
    color:#48aff0; }

.bp3-icon.bp3-intent-success, .bp3-icon-standard.bp3-intent-success, .bp3-icon-large.bp3-intent-success{
  color:#0d8050; }
  .bp3-dark .bp3-icon.bp3-intent-success, .bp3-dark .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-icon-large.bp3-intent-success{
    color:#3dcc91; }

.bp3-icon.bp3-intent-warning, .bp3-icon-standard.bp3-intent-warning, .bp3-icon-large.bp3-intent-warning{
  color:#bf7326; }
  .bp3-dark .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-icon-large.bp3-intent-warning{
    color:#ffb366; }

.bp3-icon.bp3-intent-danger, .bp3-icon-standard.bp3-intent-danger, .bp3-icon-large.bp3-intent-danger{
  color:#c23030; }
  .bp3-dark .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-icon-large.bp3-intent-danger{
    color:#ff7373; }

span.bp3-icon-standard{
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon-large{
  font-family:"Icons20", sans-serif;
  font-size:20px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon:empty{
  font-family:"Icons20";
  font-size:inherit;
  font-style:normal;
  font-weight:400;
  line-height:1; }
  span.bp3-icon:empty::before{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased; }

.bp3-icon-add::before{
  content:""; }

.bp3-icon-add-column-left::before{
  content:""; }

.bp3-icon-add-column-right::before{
  content:""; }

.bp3-icon-add-row-bottom::before{
  content:""; }

.bp3-icon-add-row-top::before{
  content:""; }

.bp3-icon-add-to-artifact::before{
  content:""; }

.bp3-icon-add-to-folder::before{
  content:""; }

.bp3-icon-airplane::before{
  content:""; }

.bp3-icon-align-center::before{
  content:""; }

.bp3-icon-align-justify::before{
  content:""; }

.bp3-icon-align-left::before{
  content:""; }

.bp3-icon-align-right::before{
  content:""; }

.bp3-icon-alignment-bottom::before{
  content:""; }

.bp3-icon-alignment-horizontal-center::before{
  content:""; }

.bp3-icon-alignment-left::before{
  content:""; }

.bp3-icon-alignment-right::before{
  content:""; }

.bp3-icon-alignment-top::before{
  content:""; }

.bp3-icon-alignment-vertical-center::before{
  content:""; }

.bp3-icon-annotation::before{
  content:""; }

.bp3-icon-application::before{
  content:""; }

.bp3-icon-applications::before{
  content:""; }

.bp3-icon-archive::before{
  content:""; }

.bp3-icon-arrow-bottom-left::before{
  content:"↙"; }

.bp3-icon-arrow-bottom-right::before{
  content:"↘"; }

.bp3-icon-arrow-down::before{
  content:"↓"; }

.bp3-icon-arrow-left::before{
  content:"←"; }

.bp3-icon-arrow-right::before{
  content:"→"; }

.bp3-icon-arrow-top-left::before{
  content:"↖"; }

.bp3-icon-arrow-top-right::before{
  content:"↗"; }

.bp3-icon-arrow-up::before{
  content:"↑"; }

.bp3-icon-arrows-horizontal::before{
  content:"↔"; }

.bp3-icon-arrows-vertical::before{
  content:"↕"; }

.bp3-icon-asterisk::before{
  content:"*"; }

.bp3-icon-automatic-updates::before{
  content:""; }

.bp3-icon-badge::before{
  content:""; }

.bp3-icon-ban-circle::before{
  content:""; }

.bp3-icon-bank-account::before{
  content:""; }

.bp3-icon-barcode::before{
  content:""; }

.bp3-icon-blank::before{
  content:""; }

.bp3-icon-blocked-person::before{
  content:""; }

.bp3-icon-bold::before{
  content:""; }

.bp3-icon-book::before{
  content:""; }

.bp3-icon-bookmark::before{
  content:""; }

.bp3-icon-box::before{
  content:""; }

.bp3-icon-briefcase::before{
  content:""; }

.bp3-icon-bring-data::before{
  content:""; }

.bp3-icon-build::before{
  content:""; }

.bp3-icon-calculator::before{
  content:""; }

.bp3-icon-calendar::before{
  content:""; }

.bp3-icon-camera::before{
  content:""; }

.bp3-icon-caret-down::before{
  content:"⌄"; }

.bp3-icon-caret-left::before{
  content:"〈"; }

.bp3-icon-caret-right::before{
  content:"〉"; }

.bp3-icon-caret-up::before{
  content:"⌃"; }

.bp3-icon-cell-tower::before{
  content:""; }

.bp3-icon-changes::before{
  content:""; }

.bp3-icon-chart::before{
  content:""; }

.bp3-icon-chat::before{
  content:""; }

.bp3-icon-chevron-backward::before{
  content:""; }

.bp3-icon-chevron-down::before{
  content:""; }

.bp3-icon-chevron-forward::before{
  content:""; }

.bp3-icon-chevron-left::before{
  content:""; }

.bp3-icon-chevron-right::before{
  content:""; }

.bp3-icon-chevron-up::before{
  content:""; }

.bp3-icon-circle::before{
  content:""; }

.bp3-icon-circle-arrow-down::before{
  content:""; }

.bp3-icon-circle-arrow-left::before{
  content:""; }

.bp3-icon-circle-arrow-right::before{
  content:""; }

.bp3-icon-circle-arrow-up::before{
  content:""; }

.bp3-icon-citation::before{
  content:""; }

.bp3-icon-clean::before{
  content:""; }

.bp3-icon-clipboard::before{
  content:""; }

.bp3-icon-cloud::before{
  content:"☁"; }

.bp3-icon-cloud-download::before{
  content:""; }

.bp3-icon-cloud-upload::before{
  content:""; }

.bp3-icon-code::before{
  content:""; }

.bp3-icon-code-block::before{
  content:""; }

.bp3-icon-cog::before{
  content:""; }

.bp3-icon-collapse-all::before{
  content:""; }

.bp3-icon-column-layout::before{
  content:""; }

.bp3-icon-comment::before{
  content:""; }

.bp3-icon-comparison::before{
  content:""; }

.bp3-icon-compass::before{
  content:""; }

.bp3-icon-compressed::before{
  content:""; }

.bp3-icon-confirm::before{
  content:""; }

.bp3-icon-console::before{
  content:""; }

.bp3-icon-contrast::before{
  content:""; }

.bp3-icon-control::before{
  content:""; }

.bp3-icon-credit-card::before{
  content:""; }

.bp3-icon-cross::before{
  content:"✗"; }

.bp3-icon-crown::before{
  content:""; }

.bp3-icon-cube::before{
  content:""; }

.bp3-icon-cube-add::before{
  content:""; }

.bp3-icon-cube-remove::before{
  content:""; }

.bp3-icon-curved-range-chart::before{
  content:""; }

.bp3-icon-cut::before{
  content:""; }

.bp3-icon-dashboard::before{
  content:""; }

.bp3-icon-data-lineage::before{
  content:""; }

.bp3-icon-database::before{
  content:""; }

.bp3-icon-delete::before{
  content:""; }

.bp3-icon-delta::before{
  content:"Δ"; }

.bp3-icon-derive-column::before{
  content:""; }

.bp3-icon-desktop::before{
  content:""; }

.bp3-icon-diagnosis::before{
  content:""; }

.bp3-icon-diagram-tree::before{
  content:""; }

.bp3-icon-direction-left::before{
  content:""; }

.bp3-icon-direction-right::before{
  content:""; }

.bp3-icon-disable::before{
  content:""; }

.bp3-icon-document::before{
  content:""; }

.bp3-icon-document-open::before{
  content:""; }

.bp3-icon-document-share::before{
  content:""; }

.bp3-icon-dollar::before{
  content:"$"; }

.bp3-icon-dot::before{
  content:"•"; }

.bp3-icon-double-caret-horizontal::before{
  content:""; }

.bp3-icon-double-caret-vertical::before{
  content:""; }

.bp3-icon-double-chevron-down::before{
  content:""; }

.bp3-icon-double-chevron-left::before{
  content:""; }

.bp3-icon-double-chevron-right::before{
  content:""; }

.bp3-icon-double-chevron-up::before{
  content:""; }

.bp3-icon-doughnut-chart::before{
  content:""; }

.bp3-icon-download::before{
  content:""; }

.bp3-icon-drag-handle-horizontal::before{
  content:""; }

.bp3-icon-drag-handle-vertical::before{
  content:""; }

.bp3-icon-draw::before{
  content:""; }

.bp3-icon-drive-time::before{
  content:""; }

.bp3-icon-duplicate::before{
  content:""; }

.bp3-icon-edit::before{
  content:"✎"; }

.bp3-icon-eject::before{
  content:"⏏"; }

.bp3-icon-endorsed::before{
  content:""; }

.bp3-icon-envelope::before{
  content:"✉"; }

.bp3-icon-equals::before{
  content:""; }

.bp3-icon-eraser::before{
  content:""; }

.bp3-icon-error::before{
  content:""; }

.bp3-icon-euro::before{
  content:"€"; }

.bp3-icon-exchange::before{
  content:""; }

.bp3-icon-exclude-row::before{
  content:""; }

.bp3-icon-expand-all::before{
  content:""; }

.bp3-icon-export::before{
  content:""; }

.bp3-icon-eye-off::before{
  content:""; }

.bp3-icon-eye-on::before{
  content:""; }

.bp3-icon-eye-open::before{
  content:""; }

.bp3-icon-fast-backward::before{
  content:""; }

.bp3-icon-fast-forward::before{
  content:""; }

.bp3-icon-feed::before{
  content:""; }

.bp3-icon-feed-subscribed::before{
  content:""; }

.bp3-icon-film::before{
  content:""; }

.bp3-icon-filter::before{
  content:""; }

.bp3-icon-filter-keep::before{
  content:""; }

.bp3-icon-filter-list::before{
  content:""; }

.bp3-icon-filter-open::before{
  content:""; }

.bp3-icon-filter-remove::before{
  content:""; }

.bp3-icon-flag::before{
  content:"⚑"; }

.bp3-icon-flame::before{
  content:""; }

.bp3-icon-flash::before{
  content:""; }

.bp3-icon-floppy-disk::before{
  content:""; }

.bp3-icon-flow-branch::before{
  content:""; }

.bp3-icon-flow-end::before{
  content:""; }

.bp3-icon-flow-linear::before{
  content:""; }

.bp3-icon-flow-review::before{
  content:""; }

.bp3-icon-flow-review-branch::before{
  content:""; }

.bp3-icon-flows::before{
  content:""; }

.bp3-icon-folder-close::before{
  content:""; }

.bp3-icon-folder-new::before{
  content:""; }

.bp3-icon-folder-open::before{
  content:""; }

.bp3-icon-folder-shared::before{
  content:""; }

.bp3-icon-folder-shared-open::before{
  content:""; }

.bp3-icon-follower::before{
  content:""; }

.bp3-icon-following::before{
  content:""; }

.bp3-icon-font::before{
  content:""; }

.bp3-icon-fork::before{
  content:""; }

.bp3-icon-form::before{
  content:""; }

.bp3-icon-full-circle::before{
  content:""; }

.bp3-icon-full-stacked-chart::before{
  content:""; }

.bp3-icon-fullscreen::before{
  content:""; }

.bp3-icon-function::before{
  content:""; }

.bp3-icon-gantt-chart::before{
  content:""; }

.bp3-icon-geolocation::before{
  content:""; }

.bp3-icon-geosearch::before{
  content:""; }

.bp3-icon-git-branch::before{
  content:""; }

.bp3-icon-git-commit::before{
  content:""; }

.bp3-icon-git-merge::before{
  content:""; }

.bp3-icon-git-new-branch::before{
  content:""; }

.bp3-icon-git-pull::before{
  content:""; }

.bp3-icon-git-push::before{
  content:""; }

.bp3-icon-git-repo::before{
  content:""; }

.bp3-icon-glass::before{
  content:""; }

.bp3-icon-globe::before{
  content:""; }

.bp3-icon-globe-network::before{
  content:""; }

.bp3-icon-graph::before{
  content:""; }

.bp3-icon-graph-remove::before{
  content:""; }

.bp3-icon-greater-than::before{
  content:""; }

.bp3-icon-greater-than-or-equal-to::before{
  content:""; }

.bp3-icon-grid::before{
  content:""; }

.bp3-icon-grid-view::before{
  content:""; }

.bp3-icon-group-objects::before{
  content:""; }

.bp3-icon-grouped-bar-chart::before{
  content:""; }

.bp3-icon-hand::before{
  content:""; }

.bp3-icon-hand-down::before{
  content:""; }

.bp3-icon-hand-left::before{
  content:""; }

.bp3-icon-hand-right::before{
  content:""; }

.bp3-icon-hand-up::before{
  content:""; }

.bp3-icon-header::before{
  content:""; }

.bp3-icon-header-one::before{
  content:""; }

.bp3-icon-header-two::before{
  content:""; }

.bp3-icon-headset::before{
  content:""; }

.bp3-icon-heart::before{
  content:"♥"; }

.bp3-icon-heart-broken::before{
  content:""; }

.bp3-icon-heat-grid::before{
  content:""; }

.bp3-icon-heatmap::before{
  content:""; }

.bp3-icon-help::before{
  content:"?"; }

.bp3-icon-helper-management::before{
  content:""; }

.bp3-icon-highlight::before{
  content:""; }

.bp3-icon-history::before{
  content:""; }

.bp3-icon-home::before{
  content:"⌂"; }

.bp3-icon-horizontal-bar-chart::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-asc::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-desc::before{
  content:""; }

.bp3-icon-horizontal-distribution::before{
  content:""; }

.bp3-icon-id-number::before{
  content:""; }

.bp3-icon-image-rotate-left::before{
  content:""; }

.bp3-icon-image-rotate-right::before{
  content:""; }

.bp3-icon-import::before{
  content:""; }

.bp3-icon-inbox::before{
  content:""; }

.bp3-icon-inbox-filtered::before{
  content:""; }

.bp3-icon-inbox-geo::before{
  content:""; }

.bp3-icon-inbox-search::before{
  content:""; }

.bp3-icon-inbox-update::before{
  content:""; }

.bp3-icon-info-sign::before{
  content:"ℹ"; }

.bp3-icon-inheritance::before{
  content:""; }

.bp3-icon-inner-join::before{
  content:""; }

.bp3-icon-insert::before{
  content:""; }

.bp3-icon-intersection::before{
  content:""; }

.bp3-icon-ip-address::before{
  content:""; }

.bp3-icon-issue::before{
  content:""; }

.bp3-icon-issue-closed::before{
  content:""; }

.bp3-icon-issue-new::before{
  content:""; }

.bp3-icon-italic::before{
  content:""; }

.bp3-icon-join-table::before{
  content:""; }

.bp3-icon-key::before{
  content:""; }

.bp3-icon-key-backspace::before{
  content:""; }

.bp3-icon-key-command::before{
  content:""; }

.bp3-icon-key-control::before{
  content:""; }

.bp3-icon-key-delete::before{
  content:""; }

.bp3-icon-key-enter::before{
  content:""; }

.bp3-icon-key-escape::before{
  content:""; }

.bp3-icon-key-option::before{
  content:""; }

.bp3-icon-key-shift::before{
  content:""; }

.bp3-icon-key-tab::before{
  content:""; }

.bp3-icon-known-vehicle::before{
  content:""; }

.bp3-icon-lab-test::before{
  content:""; }

.bp3-icon-label::before{
  content:""; }

.bp3-icon-layer::before{
  content:""; }

.bp3-icon-layers::before{
  content:""; }

.bp3-icon-layout::before{
  content:""; }

.bp3-icon-layout-auto::before{
  content:""; }

.bp3-icon-layout-balloon::before{
  content:""; }

.bp3-icon-layout-circle::before{
  content:""; }

.bp3-icon-layout-grid::before{
  content:""; }

.bp3-icon-layout-group-by::before{
  content:""; }

.bp3-icon-layout-hierarchy::before{
  content:""; }

.bp3-icon-layout-linear::before{
  content:""; }

.bp3-icon-layout-skew-grid::before{
  content:""; }

.bp3-icon-layout-sorted-clusters::before{
  content:""; }

.bp3-icon-learning::before{
  content:""; }

.bp3-icon-left-join::before{
  content:""; }

.bp3-icon-less-than::before{
  content:""; }

.bp3-icon-less-than-or-equal-to::before{
  content:""; }

.bp3-icon-lifesaver::before{
  content:""; }

.bp3-icon-lightbulb::before{
  content:""; }

.bp3-icon-link::before{
  content:""; }

.bp3-icon-list::before{
  content:"☰"; }

.bp3-icon-list-columns::before{
  content:""; }

.bp3-icon-list-detail-view::before{
  content:""; }

.bp3-icon-locate::before{
  content:""; }

.bp3-icon-lock::before{
  content:""; }

.bp3-icon-log-in::before{
  content:""; }

.bp3-icon-log-out::before{
  content:""; }

.bp3-icon-manual::before{
  content:""; }

.bp3-icon-manually-entered-data::before{
  content:""; }

.bp3-icon-map::before{
  content:""; }

.bp3-icon-map-create::before{
  content:""; }

.bp3-icon-map-marker::before{
  content:""; }

.bp3-icon-maximize::before{
  content:""; }

.bp3-icon-media::before{
  content:""; }

.bp3-icon-menu::before{
  content:""; }

.bp3-icon-menu-closed::before{
  content:""; }

.bp3-icon-menu-open::before{
  content:""; }

.bp3-icon-merge-columns::before{
  content:""; }

.bp3-icon-merge-links::before{
  content:""; }

.bp3-icon-minimize::before{
  content:""; }

.bp3-icon-minus::before{
  content:"−"; }

.bp3-icon-mobile-phone::before{
  content:""; }

.bp3-icon-mobile-video::before{
  content:""; }

.bp3-icon-moon::before{
  content:""; }

.bp3-icon-more::before{
  content:""; }

.bp3-icon-mountain::before{
  content:""; }

.bp3-icon-move::before{
  content:""; }

.bp3-icon-mugshot::before{
  content:""; }

.bp3-icon-multi-select::before{
  content:""; }

.bp3-icon-music::before{
  content:""; }

.bp3-icon-new-drawing::before{
  content:""; }

.bp3-icon-new-grid-item::before{
  content:""; }

.bp3-icon-new-layer::before{
  content:""; }

.bp3-icon-new-layers::before{
  content:""; }

.bp3-icon-new-link::before{
  content:""; }

.bp3-icon-new-object::before{
  content:""; }

.bp3-icon-new-person::before{
  content:""; }

.bp3-icon-new-prescription::before{
  content:""; }

.bp3-icon-new-text-box::before{
  content:""; }

.bp3-icon-ninja::before{
  content:""; }

.bp3-icon-not-equal-to::before{
  content:""; }

.bp3-icon-notifications::before{
  content:""; }

.bp3-icon-notifications-updated::before{
  content:""; }

.bp3-icon-numbered-list::before{
  content:""; }

.bp3-icon-numerical::before{
  content:""; }

.bp3-icon-office::before{
  content:""; }

.bp3-icon-offline::before{
  content:""; }

.bp3-icon-oil-field::before{
  content:""; }

.bp3-icon-one-column::before{
  content:""; }

.bp3-icon-outdated::before{
  content:""; }

.bp3-icon-page-layout::before{
  content:""; }

.bp3-icon-panel-stats::before{
  content:""; }

.bp3-icon-panel-table::before{
  content:""; }

.bp3-icon-paperclip::before{
  content:""; }

.bp3-icon-paragraph::before{
  content:""; }

.bp3-icon-path::before{
  content:""; }

.bp3-icon-path-search::before{
  content:""; }

.bp3-icon-pause::before{
  content:""; }

.bp3-icon-people::before{
  content:""; }

.bp3-icon-percentage::before{
  content:""; }

.bp3-icon-person::before{
  content:""; }

.bp3-icon-phone::before{
  content:"☎"; }

.bp3-icon-pie-chart::before{
  content:""; }

.bp3-icon-pin::before{
  content:""; }

.bp3-icon-pivot::before{
  content:""; }

.bp3-icon-pivot-table::before{
  content:""; }

.bp3-icon-play::before{
  content:""; }

.bp3-icon-plus::before{
  content:"+"; }

.bp3-icon-polygon-filter::before{
  content:""; }

.bp3-icon-power::before{
  content:""; }

.bp3-icon-predictive-analysis::before{
  content:""; }

.bp3-icon-prescription::before{
  content:""; }

.bp3-icon-presentation::before{
  content:""; }

.bp3-icon-print::before{
  content:"⎙"; }

.bp3-icon-projects::before{
  content:""; }

.bp3-icon-properties::before{
  content:""; }

.bp3-icon-property::before{
  content:""; }

.bp3-icon-publish-function::before{
  content:""; }

.bp3-icon-pulse::before{
  content:""; }

.bp3-icon-random::before{
  content:""; }

.bp3-icon-record::before{
  content:""; }

.bp3-icon-redo::before{
  content:""; }

.bp3-icon-refresh::before{
  content:""; }

.bp3-icon-regression-chart::before{
  content:""; }

.bp3-icon-remove::before{
  content:""; }

.bp3-icon-remove-column::before{
  content:""; }

.bp3-icon-remove-column-left::before{
  content:""; }

.bp3-icon-remove-column-right::before{
  content:""; }

.bp3-icon-remove-row-bottom::before{
  content:""; }

.bp3-icon-remove-row-top::before{
  content:""; }

.bp3-icon-repeat::before{
  content:""; }

.bp3-icon-reset::before{
  content:""; }

.bp3-icon-resolve::before{
  content:""; }

.bp3-icon-rig::before{
  content:""; }

.bp3-icon-right-join::before{
  content:""; }

.bp3-icon-ring::before{
  content:""; }

.bp3-icon-rotate-document::before{
  content:""; }

.bp3-icon-rotate-page::before{
  content:""; }

.bp3-icon-satellite::before{
  content:""; }

.bp3-icon-saved::before{
  content:""; }

.bp3-icon-scatter-plot::before{
  content:""; }

.bp3-icon-search::before{
  content:""; }

.bp3-icon-search-around::before{
  content:""; }

.bp3-icon-search-template::before{
  content:""; }

.bp3-icon-search-text::before{
  content:""; }

.bp3-icon-segmented-control::before{
  content:""; }

.bp3-icon-select::before{
  content:""; }

.bp3-icon-selection::before{
  content:"⦿"; }

.bp3-icon-send-to::before{
  content:""; }

.bp3-icon-send-to-graph::before{
  content:""; }

.bp3-icon-send-to-map::before{
  content:""; }

.bp3-icon-series-add::before{
  content:""; }

.bp3-icon-series-configuration::before{
  content:""; }

.bp3-icon-series-derived::before{
  content:""; }

.bp3-icon-series-filtered::before{
  content:""; }

.bp3-icon-series-search::before{
  content:""; }

.bp3-icon-settings::before{
  content:""; }

.bp3-icon-share::before{
  content:""; }

.bp3-icon-shield::before{
  content:""; }

.bp3-icon-shop::before{
  content:""; }

.bp3-icon-shopping-cart::before{
  content:""; }

.bp3-icon-signal-search::before{
  content:""; }

.bp3-icon-sim-card::before{
  content:""; }

.bp3-icon-slash::before{
  content:""; }

.bp3-icon-small-cross::before{
  content:""; }

.bp3-icon-small-minus::before{
  content:""; }

.bp3-icon-small-plus::before{
  content:""; }

.bp3-icon-small-tick::before{
  content:""; }

.bp3-icon-snowflake::before{
  content:""; }

.bp3-icon-social-media::before{
  content:""; }

.bp3-icon-sort::before{
  content:""; }

.bp3-icon-sort-alphabetical::before{
  content:""; }

.bp3-icon-sort-alphabetical-desc::before{
  content:""; }

.bp3-icon-sort-asc::before{
  content:""; }

.bp3-icon-sort-desc::before{
  content:""; }

.bp3-icon-sort-numerical::before{
  content:""; }

.bp3-icon-sort-numerical-desc::before{
  content:""; }

.bp3-icon-split-columns::before{
  content:""; }

.bp3-icon-square::before{
  content:""; }

.bp3-icon-stacked-chart::before{
  content:""; }

.bp3-icon-star::before{
  content:"★"; }

.bp3-icon-star-empty::before{
  content:"☆"; }

.bp3-icon-step-backward::before{
  content:""; }

.bp3-icon-step-chart::before{
  content:""; }

.bp3-icon-step-forward::before{
  content:""; }

.bp3-icon-stop::before{
  content:""; }

.bp3-icon-stopwatch::before{
  content:""; }

.bp3-icon-strikethrough::before{
  content:""; }

.bp3-icon-style::before{
  content:""; }

.bp3-icon-swap-horizontal::before{
  content:""; }

.bp3-icon-swap-vertical::before{
  content:""; }

.bp3-icon-symbol-circle::before{
  content:""; }

.bp3-icon-symbol-cross::before{
  content:""; }

.bp3-icon-symbol-diamond::before{
  content:""; }

.bp3-icon-symbol-square::before{
  content:""; }

.bp3-icon-symbol-triangle-down::before{
  content:""; }

.bp3-icon-symbol-triangle-up::before{
  content:""; }

.bp3-icon-tag::before{
  content:""; }

.bp3-icon-take-action::before{
  content:""; }

.bp3-icon-taxi::before{
  content:""; }

.bp3-icon-text-highlight::before{
  content:""; }

.bp3-icon-th::before{
  content:""; }

.bp3-icon-th-derived::before{
  content:""; }

.bp3-icon-th-disconnect::before{
  content:""; }

.bp3-icon-th-filtered::before{
  content:""; }

.bp3-icon-th-list::before{
  content:""; }

.bp3-icon-thumbs-down::before{
  content:""; }

.bp3-icon-thumbs-up::before{
  content:""; }

.bp3-icon-tick::before{
  content:"✓"; }

.bp3-icon-tick-circle::before{
  content:""; }

.bp3-icon-time::before{
  content:"⏲"; }

.bp3-icon-timeline-area-chart::before{
  content:""; }

.bp3-icon-timeline-bar-chart::before{
  content:""; }

.bp3-icon-timeline-events::before{
  content:""; }

.bp3-icon-timeline-line-chart::before{
  content:""; }

.bp3-icon-tint::before{
  content:""; }

.bp3-icon-torch::before{
  content:""; }

.bp3-icon-tractor::before{
  content:""; }

.bp3-icon-train::before{
  content:""; }

.bp3-icon-translate::before{
  content:""; }

.bp3-icon-trash::before{
  content:""; }

.bp3-icon-tree::before{
  content:""; }

.bp3-icon-trending-down::before{
  content:""; }

.bp3-icon-trending-up::before{
  content:""; }

.bp3-icon-truck::before{
  content:""; }

.bp3-icon-two-columns::before{
  content:""; }

.bp3-icon-unarchive::before{
  content:""; }

.bp3-icon-underline::before{
  content:"⎁"; }

.bp3-icon-undo::before{
  content:"⎌"; }

.bp3-icon-ungroup-objects::before{
  content:""; }

.bp3-icon-unknown-vehicle::before{
  content:""; }

.bp3-icon-unlock::before{
  content:""; }

.bp3-icon-unpin::before{
  content:""; }

.bp3-icon-unresolve::before{
  content:""; }

.bp3-icon-updated::before{
  content:""; }

.bp3-icon-upload::before{
  content:""; }

.bp3-icon-user::before{
  content:""; }

.bp3-icon-variable::before{
  content:""; }

.bp3-icon-vertical-bar-chart-asc::before{
  content:""; }

.bp3-icon-vertical-bar-chart-desc::before{
  content:""; }

.bp3-icon-vertical-distribution::before{
  content:""; }

.bp3-icon-video::before{
  content:""; }

.bp3-icon-volume-down::before{
  content:""; }

.bp3-icon-volume-off::before{
  content:""; }

.bp3-icon-volume-up::before{
  content:""; }

.bp3-icon-walk::before{
  content:""; }

.bp3-icon-warning-sign::before{
  content:""; }

.bp3-icon-waterfall-chart::before{
  content:""; }

.bp3-icon-widget::before{
  content:""; }

.bp3-icon-widget-button::before{
  content:""; }

.bp3-icon-widget-footer::before{
  content:""; }

.bp3-icon-widget-header::before{
  content:""; }

.bp3-icon-wrench::before{
  content:""; }

.bp3-icon-zoom-in::before{
  content:""; }

.bp3-icon-zoom-out::before{
  content:""; }

.bp3-icon-zoom-to-fit::before{
  content:""; }
.bp3-submenu > .bp3-popover-wrapper{
  display:block; }

.bp3-submenu .bp3-popover-target{
  display:block; }
  .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{ }

.bp3-submenu.bp3-popover{
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0 5px; }
  .bp3-submenu.bp3-popover > .bp3-popover-content{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-submenu.bp3-popover, .bp3-submenu.bp3-popover.bp3-dark{
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-dark .bp3-submenu.bp3-popover > .bp3-popover-content, .bp3-submenu.bp3-popover.bp3-dark > .bp3-popover-content{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
.bp3-menu{
  background:#ffffff;
  border-radius:3px;
  color:#182026;
  list-style:none;
  margin:0;
  min-width:180px;
  padding:5px;
  text-align:left; }

.bp3-menu-divider{
  border-top:1px solid rgba(16, 22, 26, 0.15);
  display:block;
  margin:5px; }
  .bp3-dark .bp3-menu-divider{
    border-top-color:rgba(255, 255, 255, 0.15); }

.bp3-menu-item{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  border-radius:2px;
  color:inherit;
  line-height:20px;
  padding:5px 7px;
  text-decoration:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-menu-item > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-menu-item > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-menu-item::before,
  .bp3-menu-item > *{
    margin-right:7px; }
  .bp3-menu-item:empty::before,
  .bp3-menu-item > :last-child{
    margin-right:0; }
  .bp3-menu-item > .bp3-fill{
    word-break:break-word; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    background-color:rgba(167, 182, 194, 0.3);
    cursor:pointer;
    text-decoration:none; }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-dark .bp3-menu-item{
    color:inherit; }
    .bp3-dark .bp3-menu-item:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
      background-color:rgba(138, 155, 168, 0.15);
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-disabled{
      background-color:inherit;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-menu-item.bp3-intent-primary{
    color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-primary::before, .bp3-menu-item.bp3-intent-primary::after,
    .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary:active, .bp3-menu-item.bp3-intent-primary:active::before, .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-success{
    color:#0d8050; }
    .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-success::before, .bp3-menu-item.bp3-intent-success::after,
    .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-menu-item.bp3-intent-success:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success:active, .bp3-menu-item.bp3-intent-success:active::before, .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-warning{
    color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-warning::before, .bp3-menu-item.bp3-intent-warning::after,
    .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning:active, .bp3-menu-item.bp3-intent-warning:active::before, .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-danger{
    color:#c23030; }
    .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-danger::before, .bp3-menu-item.bp3-intent-danger::after,
    .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger:active, .bp3-menu-item.bp3-intent-danger:active::before, .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    margin-right:7px; }
  .bp3-menu-item::before,
  .bp3-menu-item > .bp3-icon{
    color:#5c7080;
    margin-top:2px; }
  .bp3-menu-item .bp3-menu-item-label{
    color:#5c7080; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    color:inherit; }
  .bp3-menu-item.bp3-active, .bp3-menu-item:active{
    background-color:rgba(115, 134, 148, 0.3); }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit !important;
    color:rgba(92, 112, 128, 0.6) !important;
    cursor:not-allowed !important;
    outline:none !important; }
    .bp3-menu-item.bp3-disabled::before,
    .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-large .bp3-menu-item{
    font-size:16px;
    line-height:22px;
    padding:9px 7px; }
    .bp3-large .bp3-menu-item .bp3-icon{
      margin-top:3px; }
    .bp3-large .bp3-menu-item::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      margin-right:10px;
      margin-top:1px; }

button.bp3-menu-item{
  background:none;
  border:none;
  text-align:left;
  width:100%; }
.bp3-menu-header{
  border-top:1px solid rgba(16, 22, 26, 0.15);
  display:block;
  margin:5px;
  cursor:default;
  padding-left:2px; }
  .bp3-dark .bp3-menu-header{
    border-top-color:rgba(255, 255, 255, 0.15); }
  .bp3-menu-header:first-of-type{
    border-top:none; }
  .bp3-menu-header > h6{
    color:#182026;
    font-weight:600;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    line-height:17px;
    margin:0;
    padding:10px 7px 0 1px; }
    .bp3-dark .bp3-menu-header > h6{
      color:#f5f8fa; }
  .bp3-menu-header:first-of-type > h6{
    padding-top:0; }
  .bp3-large .bp3-menu-header > h6{
    font-size:18px;
    padding-bottom:5px;
    padding-top:15px; }
  .bp3-large .bp3-menu-header:first-of-type > h6{
    padding-top:0; }

.bp3-dark .bp3-menu{
  background:#30404d;
  color:#f5f8fa; }

.bp3-dark .bp3-menu-item{ }
  .bp3-dark .bp3-menu-item.bp3-intent-primary{
    color:#48aff0; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary::before, .bp3-dark .bp3-menu-item.bp3-intent-primary::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#48aff0; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary:active, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-success{
    color:#3dcc91; }
    .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-success::before, .bp3-dark .bp3-menu-item.bp3-intent-success::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#3dcc91; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success:active, .bp3-dark .bp3-menu-item.bp3-intent-success:active::before, .bp3-dark .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning{
    color:#ffb366; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning::before, .bp3-dark .bp3-menu-item.bp3-intent-warning::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#ffb366; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning:active, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger{
    color:#ff7373; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger::before, .bp3-dark .bp3-menu-item.bp3-intent-danger::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#ff7373; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger:active, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item::before,
  .bp3-dark .bp3-menu-item > .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-menu-item .bp3-menu-item-label{
    color:#a7b6c2; }
  .bp3-dark .bp3-menu-item.bp3-active, .bp3-dark .bp3-menu-item:active{
    background-color:rgba(138, 155, 168, 0.3); }
  .bp3-dark .bp3-menu-item.bp3-disabled{
    color:rgba(167, 182, 194, 0.6) !important; }
    .bp3-dark .bp3-menu-item.bp3-disabled::before,
    .bp3-dark .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-dark .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(167, 182, 194, 0.6) !important; }

.bp3-dark .bp3-menu-divider,
.bp3-dark .bp3-menu-header{
  border-color:rgba(255, 255, 255, 0.15); }

.bp3-dark .bp3-menu-header > h6{
  color:#f5f8fa; }

.bp3-label .bp3-menu{
  margin-top:5px; }
.bp3-navbar{
  background-color:#ffffff;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  height:50px;
  padding:0 15px;
  position:relative;
  width:100%;
  z-index:10; }
  .bp3-navbar.bp3-dark,
  .bp3-dark .bp3-navbar{
    background-color:#394b59; }
  .bp3-navbar.bp3-dark{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-navbar{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-navbar.bp3-fixed-top{
    left:0;
    position:fixed;
    right:0;
    top:0; }

.bp3-navbar-heading{
  font-size:16px;
  margin-right:15px; }

.bp3-navbar-group{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:50px; }
  .bp3-navbar-group.bp3-align-left{
    float:left; }
  .bp3-navbar-group.bp3-align-right{
    float:right; }

.bp3-navbar-divider{
  border-left:1px solid rgba(16, 22, 26, 0.15);
  height:20px;
  margin:0 10px; }
  .bp3-dark .bp3-navbar-divider{
    border-left-color:rgba(255, 255, 255, 0.15); }
.bp3-non-ideal-state{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  height:100%;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  text-align:center;
  width:100%; }
  .bp3-non-ideal-state > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-non-ideal-state > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-non-ideal-state::before,
  .bp3-non-ideal-state > *{
    margin-bottom:20px; }
  .bp3-non-ideal-state:empty::before,
  .bp3-non-ideal-state > :last-child{
    margin-bottom:0; }
  .bp3-non-ideal-state > *{
    max-width:400px; }

.bp3-non-ideal-state-visual{
  color:rgba(92, 112, 128, 0.6);
  font-size:60px; }
  .bp3-dark .bp3-non-ideal-state-visual{
    color:rgba(167, 182, 194, 0.6); }

.bp3-overflow-list{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:nowrap;
      flex-wrap:nowrap;
  min-width:0; }

.bp3-overflow-list-spacer{
  -ms-flex-negative:1;
      flex-shrink:1;
  width:1px; }

body.bp3-overlay-open{
  overflow:hidden; }

.bp3-overlay{
  bottom:0;
  left:0;
  position:static;
  right:0;
  top:0;
  z-index:20; }
  .bp3-overlay:not(.bp3-overlay-open){
    pointer-events:none; }
  .bp3-overlay.bp3-overlay-container{
    overflow:hidden;
    position:fixed; }
    .bp3-overlay.bp3-overlay-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-scroll-container{
    overflow:auto;
    position:fixed; }
    .bp3-overlay.bp3-overlay-scroll-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-inline{
    display:inline;
    overflow:visible; }

.bp3-overlay-content{
  position:fixed;
  z-index:20; }
  .bp3-overlay-inline .bp3-overlay-content,
  .bp3-overlay-scroll-container .bp3-overlay-content{
    position:absolute; }

.bp3-overlay-backdrop{
  bottom:0;
  left:0;
  position:fixed;
  right:0;
  top:0;
  opacity:1;
  background-color:rgba(16, 22, 26, 0.7);
  overflow:auto;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none;
  z-index:20; }
  .bp3-overlay-backdrop.bp3-overlay-enter, .bp3-overlay-backdrop.bp3-overlay-appear{
    opacity:0; }
  .bp3-overlay-backdrop.bp3-overlay-enter-active, .bp3-overlay-backdrop.bp3-overlay-appear-active{
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-overlay-backdrop.bp3-overlay-exit{
    opacity:1; }
  .bp3-overlay-backdrop.bp3-overlay-exit-active{
    opacity:0;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-overlay-backdrop:focus{
    outline:none; }
  .bp3-overlay-inline .bp3-overlay-backdrop{
    position:absolute; }
.bp3-panel-stack{
  overflow:hidden;
  position:relative; }

.bp3-panel-stack-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  height:30px;
  z-index:1; }
  .bp3-dark .bp3-panel-stack-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack-header > span{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1; }
  .bp3-panel-stack-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack-view{
  bottom:0;
  left:0;
  position:absolute;
  right:0;
  top:0;
  background-color:#ffffff;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  overflow-y:auto;
  z-index:1; }
  .bp3-dark .bp3-panel-stack-view{
    background-color:#30404d; }
  .bp3-panel-stack-view:nth-last-child(n + 4){
    display:none; }

.bp3-panel-stack-push .bp3-panel-stack-enter, .bp3-panel-stack-push .bp3-panel-stack-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack-push .bp3-panel-stack-enter-active, .bp3-panel-stack-push .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-push .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-push .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-enter, .bp3-panel-stack-pop .bp3-panel-stack-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack-pop .bp3-panel-stack-enter-active, .bp3-panel-stack-pop .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-pop .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }
.bp3-panel-stack2{
  overflow:hidden;
  position:relative; }

.bp3-panel-stack2-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  height:30px;
  z-index:1; }
  .bp3-dark .bp3-panel-stack2-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack2-header > span{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1; }
  .bp3-panel-stack2-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack2-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack2-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack2-view{
  bottom:0;
  left:0;
  position:absolute;
  right:0;
  top:0;
  background-color:#ffffff;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  overflow-y:auto;
  z-index:1; }
  .bp3-dark .bp3-panel-stack2-view{
    background-color:#30404d; }
  .bp3-panel-stack2-view:nth-last-child(n + 4){
    display:none; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter, .bp3-panel-stack2-push .bp3-panel-stack2-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter-active, .bp3-panel-stack2-push .bp3-panel-stack2-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter, .bp3-panel-stack2-pop .bp3-panel-stack2-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter-active, .bp3-panel-stack2-pop .bp3-panel-stack2-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }
.bp3-popover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1);
  border-radius:3px;
  display:inline-block;
  z-index:20; }
  .bp3-popover .bp3-popover-arrow{
    height:30px;
    position:absolute;
    width:30px; }
    .bp3-popover .bp3-popover-arrow::before{
      height:20px;
      margin:5px;
      width:20px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover{
    margin-bottom:17px;
    margin-top:-17px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
      bottom:-11px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover{
    margin-left:17px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
      left:-11px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover{
    margin-top:17px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
      top:-11px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover{
    margin-left:-17px;
    margin-right:17px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
      right:-11px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-popover > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-popover > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
    top:-0.3934px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
    right:-0.3934px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
    left:-0.3934px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
    bottom:-0.3934px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-popover .bp3-popover-content{
    background:#ffffff;
    color:inherit; }
  .bp3-popover .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-popover .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-popover .bp3-popover-arrow-fill{
    fill:#ffffff; }
  .bp3-popover-enter > .bp3-popover, .bp3-popover-appear > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3); }
  .bp3-popover-enter-active > .bp3-popover, .bp3-popover-appear-active > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-popover-exit > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-popover .bp3-popover-content{
    border-radius:3px;
    position:relative; }
  .bp3-popover.bp3-popover-content-sizing .bp3-popover-content{
    max-width:350px;
    padding:20px; }
  .bp3-popover-target + .bp3-overlay .bp3-popover.bp3-popover-content-sizing{
    width:350px; }
  .bp3-popover.bp3-minimal{
    margin:0 !important; }
    .bp3-popover.bp3-minimal .bp3-popover-arrow{
      display:none; }
    .bp3-popover.bp3-minimal.bp3-popover{
      -webkit-transform:scale(1);
              transform:scale(1); }
      .bp3-popover-enter > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-enter-active > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-delay:0;
                transition-delay:0;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
      .bp3-popover-exit > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-exit-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-delay:0;
                transition-delay:0;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-popover.bp3-dark,
  .bp3-dark .bp3-popover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-popover .bp3-popover-content{
      background:#30404d;
      color:inherit; }
    .bp3-popover.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-popover .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-popover .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-popover.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-popover .bp3-popover-arrow-fill{
      fill:#30404d; }

.bp3-popover-arrow::before{
  border-radius:2px;
  content:"";
  display:block;
  position:absolute;
  -webkit-transform:rotate(45deg);
          transform:rotate(45deg); }

.bp3-tether-pinned .bp3-popover-arrow{
  display:none; }

.bp3-popover-backdrop{
  background:rgba(255, 255, 255, 0); }

.bp3-transition-container{
  opacity:1;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  z-index:20; }
  .bp3-transition-container.bp3-popover-enter, .bp3-transition-container.bp3-popover-appear{
    opacity:0; }
  .bp3-transition-container.bp3-popover-enter-active, .bp3-transition-container.bp3-popover-appear-active{
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-transition-container.bp3-popover-exit{
    opacity:1; }
  .bp3-transition-container.bp3-popover-exit-active{
    opacity:0;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-transition-container:focus{
    outline:none; }
  .bp3-transition-container.bp3-popover-leave .bp3-popover-content{
    pointer-events:none; }
  .bp3-transition-container[data-x-out-of-boundaries]{
    display:none; }

span.bp3-popover-target{
  display:inline-block; }

.bp3-popover-wrapper.bp3-fill{
  width:100%; }

.bp3-portal{
  left:0;
  position:absolute;
  right:0;
  top:0; }
@-webkit-keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }
@keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }

.bp3-progress-bar{
  background:rgba(92, 112, 128, 0.2);
  border-radius:40px;
  display:block;
  height:8px;
  overflow:hidden;
  position:relative;
  width:100%; }
  .bp3-progress-bar .bp3-progress-meter{
    background:linear-gradient(-45deg, rgba(255, 255, 255, 0.2) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.2) 50%, rgba(255, 255, 255, 0.2) 75%, transparent 75%);
    background-color:rgba(92, 112, 128, 0.8);
    background-size:30px 30px;
    border-radius:40px;
    height:100%;
    position:absolute;
    -webkit-transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    width:100%; }
  .bp3-progress-bar:not(.bp3-no-animation):not(.bp3-no-stripes) .bp3-progress-meter{
    animation:linear-progress-bar-stripes 300ms linear infinite reverse; }
  .bp3-progress-bar.bp3-no-stripes .bp3-progress-meter{
    background-image:none; }

.bp3-dark .bp3-progress-bar{
  background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-progress-bar .bp3-progress-meter{
    background-color:#8a9ba8; }

.bp3-progress-bar.bp3-intent-primary .bp3-progress-meter{
  background-color:#137cbd; }

.bp3-progress-bar.bp3-intent-success .bp3-progress-meter{
  background-color:#0f9960; }

.bp3-progress-bar.bp3-intent-warning .bp3-progress-meter{
  background-color:#d9822b; }

.bp3-progress-bar.bp3-intent-danger .bp3-progress-meter{
  background-color:#db3737; }
@-webkit-keyframes skeleton-glow{
  from{
    background:rgba(206, 217, 224, 0.2);
    border-color:rgba(206, 217, 224, 0.2); }
  to{
    background:rgba(92, 112, 128, 0.2);
    border-color:rgba(92, 112, 128, 0.2); } }
@keyframes skeleton-glow{
  from{
    background:rgba(206, 217, 224, 0.2);
    border-color:rgba(206, 217, 224, 0.2); }
  to{
    background:rgba(92, 112, 128, 0.2);
    border-color:rgba(92, 112, 128, 0.2); } }
.bp3-skeleton{
  -webkit-animation:1000ms linear infinite alternate skeleton-glow;
          animation:1000ms linear infinite alternate skeleton-glow;
  background:rgba(206, 217, 224, 0.2);
  background-clip:padding-box !important;
  border-color:rgba(206, 217, 224, 0.2) !important;
  border-radius:2px;
  -webkit-box-shadow:none !important;
          box-shadow:none !important;
  color:transparent !important;
  cursor:default;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-skeleton::before, .bp3-skeleton::after,
  .bp3-skeleton *{
    visibility:hidden !important; }
.bp3-slider{
  height:40px;
  min-width:150px;
  width:100%;
  cursor:default;
  outline:none;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-slider:hover{
    cursor:pointer; }
  .bp3-slider:active{
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-slider.bp3-disabled{
    cursor:not-allowed;
    opacity:0.5; }
  .bp3-slider.bp3-slider-unlabeled{
    height:16px; }

.bp3-slider-track,
.bp3-slider-progress{
  height:6px;
  left:0;
  right:0;
  top:5px;
  position:absolute; }

.bp3-slider-track{
  border-radius:3px;
  overflow:hidden; }

.bp3-slider-progress{
  background:rgba(92, 112, 128, 0.2); }
  .bp3-dark .bp3-slider-progress{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-slider-progress.bp3-intent-primary{
    background-color:#137cbd; }
  .bp3-slider-progress.bp3-intent-success{
    background-color:#0f9960; }
  .bp3-slider-progress.bp3-intent-warning{
    background-color:#d9822b; }
  .bp3-slider-progress.bp3-intent-danger{
    background-color:#db3737; }

.bp3-slider-handle{
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  color:#182026;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
  cursor:pointer;
  height:16px;
  left:0;
  position:absolute;
  top:0;
  width:16px; }
  .bp3-slider-handle:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-slider-handle:active, .bp3-slider-handle.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-slider-handle:disabled, .bp3-slider-handle.bp3-disabled{
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    outline:none; }
    .bp3-slider-handle:disabled.bp3-active, .bp3-slider-handle:disabled.bp3-active:hover, .bp3-slider-handle.bp3-disabled.bp3-active, .bp3-slider-handle.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }
  .bp3-slider-handle:focus{
    z-index:1; }
  .bp3-slider-handle:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
    cursor:-webkit-grab;
    cursor:grab;
    z-index:2; }
  .bp3-slider-handle.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-disabled .bp3-slider-handle{
    background:#bfccd6;
    -webkit-box-shadow:none;
            box-shadow:none;
    pointer-events:none; }
  .bp3-dark .bp3-slider-handle{
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover, .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-slider-handle:disabled, .bp3-dark .bp3-slider-handle.bp3-disabled{
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-slider-handle:disabled.bp3-active, .bp3-dark .bp3-slider-handle.bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-slider-handle .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-slider-handle, .bp3-dark .bp3-slider-handle:hover{
      background-color:#394b59; }
    .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#293742; }
  .bp3-dark .bp3-disabled .bp3-slider-handle{
    background:#5c7080;
    border-color:#5c7080;
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-slider-handle .bp3-slider-label{
    background:#394b59;
    border-radius:3px;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
    color:#f5f8fa;
    margin-left:8px; }
    .bp3-dark .bp3-slider-handle .bp3-slider-label{
      background:#e1e8ed;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
      color:#394b59; }
    .bp3-disabled .bp3-slider-handle .bp3-slider-label{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-slider-handle.bp3-start, .bp3-slider-handle.bp3-end{
    width:8px; }
  .bp3-slider-handle.bp3-start{
    border-bottom-right-radius:0;
    border-top-right-radius:0; }
  .bp3-slider-handle.bp3-end{
    border-bottom-left-radius:0;
    border-top-left-radius:0;
    margin-left:8px; }
    .bp3-slider-handle.bp3-end .bp3-slider-label{
      margin-left:0; }

.bp3-slider-label{
  -webkit-transform:translate(-50%, 20px);
          transform:translate(-50%, 20px);
  display:inline-block;
  font-size:12px;
  line-height:1;
  padding:2px 5px;
  position:absolute;
  vertical-align:top; }

.bp3-slider.bp3-vertical{
  height:150px;
  min-width:40px;
  width:40px; }
  .bp3-slider.bp3-vertical .bp3-slider-track,
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    bottom:0;
    height:auto;
    left:5px;
    top:0;
    width:6px; }
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    top:auto; }
  .bp3-slider.bp3-vertical .bp3-slider-label{
    -webkit-transform:translate(20px, 50%);
            transform:translate(20px, 50%); }
  .bp3-slider.bp3-vertical .bp3-slider-handle{
    top:auto; }
    .bp3-slider.bp3-vertical .bp3-slider-handle .bp3-slider-label{
      margin-left:0;
      margin-top:-8px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end, .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      height:8px;
      margin-left:0;
      width:16px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      border-bottom-right-radius:3px;
      border-top-left-radius:0; }
      .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start .bp3-slider-label{
        -webkit-transform:translate(20px);
                transform:translate(20px); }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end{
      border-bottom-left-radius:0;
      border-bottom-right-radius:0;
      border-top-left-radius:3px;
      margin-bottom:8px; }

@-webkit-keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

@keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

.bp3-spinner{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  overflow:visible;
  vertical-align:middle; }
  .bp3-spinner svg{
    display:block; }
  .bp3-spinner path{
    fill-opacity:0; }
  .bp3-spinner .bp3-spinner-head{
    stroke:rgba(92, 112, 128, 0.8);
    stroke-linecap:round;
    -webkit-transform-origin:center;
            transform-origin:center;
    -webkit-transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-spinner .bp3-spinner-track{
    stroke:rgba(92, 112, 128, 0.2); }

.bp3-spinner-animation{
  -webkit-animation:pt-spinner-animation 500ms linear infinite;
          animation:pt-spinner-animation 500ms linear infinite; }
  .bp3-no-spin > .bp3-spinner-animation{
    -webkit-animation:none;
            animation:none; }

.bp3-dark .bp3-spinner .bp3-spinner-head{
  stroke:#8a9ba8; }

.bp3-dark .bp3-spinner .bp3-spinner-track{
  stroke:rgba(16, 22, 26, 0.5); }

.bp3-spinner.bp3-intent-primary .bp3-spinner-head{
  stroke:#137cbd; }

.bp3-spinner.bp3-intent-success .bp3-spinner-head{
  stroke:#0f9960; }

.bp3-spinner.bp3-intent-warning .bp3-spinner-head{
  stroke:#d9822b; }

.bp3-spinner.bp3-intent-danger .bp3-spinner-head{
  stroke:#db3737; }
.bp3-tabs.bp3-vertical{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-tabs.bp3-vertical > .bp3-tab-list{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start;
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab{
      border-radius:3px;
      padding:0 10px;
      width:100%; }
      .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab[aria-selected="true"]{
        background-color:rgba(19, 124, 189, 0.2);
        -webkit-box-shadow:none;
                box-shadow:none; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab-indicator-wrapper .bp3-tab-indicator{
      background-color:rgba(19, 124, 189, 0.2);
      border-radius:3px;
      bottom:0;
      height:auto;
      left:0;
      right:0;
      top:0; }
  .bp3-tabs.bp3-vertical > .bp3-tab-panel{
    margin-top:0;
    padding-left:20px; }

.bp3-tab-list{
  -webkit-box-align:end;
      -ms-flex-align:end;
          align-items:flex-end;
  border:none;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  list-style:none;
  margin:0;
  padding:0;
  position:relative; }
  .bp3-tab-list > *:not(:last-child){
    margin-right:20px; }

.bp3-tab{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  color:#182026;
  cursor:pointer;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  font-size:14px;
  line-height:30px;
  max-width:100%;
  position:relative;
  vertical-align:top; }
  .bp3-tab a{
    color:inherit;
    display:block;
    text-decoration:none; }
  .bp3-tab-indicator-wrapper ~ .bp3-tab{
    background-color:transparent !important;
    -webkit-box-shadow:none !important;
            box-shadow:none !important; }
  .bp3-tab[aria-disabled="true"]{
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-tab[aria-selected="true"]{
    border-radius:0;
    -webkit-box-shadow:inset 0 -3px 0 #106ba3;
            box-shadow:inset 0 -3px 0 #106ba3; }
  .bp3-tab[aria-selected="true"], .bp3-tab:not([aria-disabled="true"]):hover{
    color:#106ba3; }
  .bp3-tab:focus{
    -moz-outline-radius:0; }
  .bp3-large > .bp3-tab{
    font-size:16px;
    line-height:40px; }

.bp3-tab-panel{
  margin-top:20px; }
  .bp3-tab-panel[aria-hidden="true"]{
    display:none; }

.bp3-tab-indicator-wrapper{
  left:0;
  pointer-events:none;
  position:absolute;
  top:0;
  -webkit-transform:translateX(0), translateY(0);
          transform:translateX(0), translateY(0);
  -webkit-transition:height, width, -webkit-transform;
  transition:height, width, -webkit-transform;
  transition:height, transform, width;
  transition:height, transform, width, -webkit-transform;
  -webkit-transition-duration:200ms;
          transition-duration:200ms;
  -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
          transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tab-indicator-wrapper .bp3-tab-indicator{
    background-color:#106ba3;
    bottom:0;
    height:3px;
    left:0;
    position:absolute;
    right:0; }
  .bp3-tab-indicator-wrapper.bp3-no-animation{
    -webkit-transition:none;
    transition:none; }

.bp3-dark .bp3-tab{
  color:#f5f8fa; }
  .bp3-dark .bp3-tab[aria-disabled="true"]{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tab[aria-selected="true"]{
    -webkit-box-shadow:inset 0 -3px 0 #48aff0;
            box-shadow:inset 0 -3px 0 #48aff0; }
  .bp3-dark .bp3-tab[aria-selected="true"], .bp3-dark .bp3-tab:not([aria-disabled="true"]):hover{
    color:#48aff0; }

.bp3-dark .bp3-tab-indicator{
  background-color:#48aff0; }

.bp3-flex-expander{
  -webkit-box-flex:1;
      -ms-flex:1 1;
          flex:1 1; }
.bp3-tag{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:#5c7080;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:none;
          box-shadow:none;
  color:#f5f8fa;
  font-size:12px;
  line-height:16px;
  max-width:100%;
  min-height:20px;
  min-width:20px;
  padding:2px 6px;
  position:relative; }
  .bp3-tag.bp3-interactive{
    cursor:pointer; }
    .bp3-tag.bp3-interactive:hover{
      background-color:rgba(92, 112, 128, 0.85); }
    .bp3-tag.bp3-interactive.bp3-active, .bp3-tag.bp3-interactive:active{
      background-color:rgba(92, 112, 128, 0.7); }
  .bp3-tag > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag::before,
  .bp3-tag > *{
    margin-right:4px; }
  .bp3-tag:empty::before,
  .bp3-tag > :last-child{
    margin-right:0; }
  .bp3-tag:focus{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:0;
    -moz-outline-radius:6px; }
  .bp3-tag.bp3-round{
    border-radius:30px;
    padding-left:8px;
    padding-right:8px; }
  .bp3-dark .bp3-tag{
    background-color:#bfccd6;
    color:#182026; }
    .bp3-dark .bp3-tag.bp3-interactive{
      cursor:pointer; }
      .bp3-dark .bp3-tag.bp3-interactive:hover{
        background-color:rgba(191, 204, 214, 0.85); }
      .bp3-dark .bp3-tag.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-interactive:active{
        background-color:rgba(191, 204, 214, 0.7); }
    .bp3-dark .bp3-tag > .bp3-icon, .bp3-dark .bp3-tag .bp3-icon-standard, .bp3-dark .bp3-tag .bp3-icon-large{
      fill:currentColor; }
  .bp3-tag > .bp3-icon, .bp3-tag .bp3-icon-standard, .bp3-tag .bp3-icon-large{
    fill:#ffffff; }
  .bp3-tag.bp3-large,
  .bp3-large .bp3-tag{
    font-size:14px;
    line-height:20px;
    min-height:30px;
    min-width:30px;
    padding:5px 10px; }
    .bp3-tag.bp3-large::before,
    .bp3-tag.bp3-large > *,
    .bp3-large .bp3-tag::before,
    .bp3-large .bp3-tag > *{
      margin-right:7px; }
    .bp3-tag.bp3-large:empty::before,
    .bp3-tag.bp3-large > :last-child,
    .bp3-large .bp3-tag:empty::before,
    .bp3-large .bp3-tag > :last-child{
      margin-right:0; }
    .bp3-tag.bp3-large.bp3-round,
    .bp3-large .bp3-tag.bp3-round{
      padding-left:12px;
      padding-right:12px; }
  .bp3-tag.bp3-intent-primary{
    background:#137cbd;
    color:#ffffff; }
    .bp3-tag.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.85); }
      .bp3-tag.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.7); }
  .bp3-tag.bp3-intent-success{
    background:#0f9960;
    color:#ffffff; }
    .bp3-tag.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.85); }
      .bp3-tag.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.7); }
  .bp3-tag.bp3-intent-warning{
    background:#d9822b;
    color:#ffffff; }
    .bp3-tag.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.85); }
      .bp3-tag.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.7); }
  .bp3-tag.bp3-intent-danger{
    background:#db3737;
    color:#ffffff; }
    .bp3-tag.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.85); }
      .bp3-tag.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.7); }
  .bp3-tag.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-tag.bp3-minimal > .bp3-icon, .bp3-tag.bp3-minimal .bp3-icon-standard, .bp3-tag.bp3-minimal .bp3-icon-large{
    fill:#5c7080; }
  .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
    background-color:rgba(138, 155, 168, 0.2);
    color:#182026; }
    .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
        background-color:rgba(92, 112, 128, 0.3); }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
        background-color:rgba(92, 112, 128, 0.4); }
    .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
      color:#f5f8fa; }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
          background-color:rgba(191, 204, 214, 0.3); }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
          background-color:rgba(191, 204, 214, 0.4); }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) > .bp3-icon, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-large{
        fill:#a7b6c2; }
  .bp3-tag.bp3-minimal.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15);
    color:#106ba3; }
    .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-primary > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-large{
      fill:#137cbd; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25);
      color:#48aff0; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
          background-color:rgba(19, 124, 189, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
          background-color:rgba(19, 124, 189, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15);
    color:#0d8050; }
    .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-success > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-large{
      fill:#0f9960; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25);
      color:#3dcc91; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
          background-color:rgba(15, 153, 96, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
          background-color:rgba(15, 153, 96, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15);
    color:#bf7326; }
    .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-warning > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-large{
      fill:#d9822b; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25);
      color:#ffb366; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
          background-color:rgba(217, 130, 43, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
          background-color:rgba(217, 130, 43, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15);
    color:#c23030; }
    .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-danger > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-large{
      fill:#db3737; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25);
      color:#ff7373; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
          background-color:rgba(219, 55, 55, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
          background-color:rgba(219, 55, 55, 0.45); }

.bp3-tag-remove{
  background:none;
  border:none;
  color:inherit;
  cursor:pointer;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin-bottom:-2px;
  margin-right:-6px !important;
  margin-top:-2px;
  opacity:0.5;
  padding:2px;
  padding-left:0; }
  .bp3-tag-remove:hover{
    background:none;
    opacity:0.8;
    text-decoration:none; }
  .bp3-tag-remove:active{
    opacity:1; }
  .bp3-tag-remove:empty::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    content:""; }
  .bp3-large .bp3-tag-remove{
    margin-right:-10px !important;
    padding:0 5px 0 0; }
    .bp3-large .bp3-tag-remove:empty::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1; }
.bp3-tag-input{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  cursor:text;
  height:auto;
  line-height:inherit;
  min-height:30px;
  padding-left:5px;
  padding-right:0; }
  .bp3-tag-input > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag-input > .bp3-tag-input-values{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag-input .bp3-tag-input-icon{
    color:#5c7080;
    margin-left:2px;
    margin-right:7px;
    margin-top:7px; }
  .bp3-tag-input .bp3-tag-input-values{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row;
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    -ms-flex-item-align:stretch;
        align-self:stretch;
    -ms-flex-wrap:wrap;
        flex-wrap:wrap;
    margin-right:7px;
    margin-top:5px;
    min-width:0; }
    .bp3-tag-input .bp3-tag-input-values > *{
      -webkit-box-flex:0;
          -ms-flex-positive:0;
              flex-grow:0;
      -ms-flex-negative:0;
          flex-shrink:0; }
    .bp3-tag-input .bp3-tag-input-values > .bp3-fill{
      -webkit-box-flex:1;
          -ms-flex-positive:1;
              flex-grow:1;
      -ms-flex-negative:1;
          flex-shrink:1; }
    .bp3-tag-input .bp3-tag-input-values::before,
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-right:5px; }
    .bp3-tag-input .bp3-tag-input-values:empty::before,
    .bp3-tag-input .bp3-tag-input-values > :last-child{
      margin-right:0; }
    .bp3-tag-input .bp3-tag-input-values:first-child .bp3-input-ghost:first-child{
      padding-left:5px; }
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-bottom:5px; }
  .bp3-tag-input .bp3-tag{
    overflow-wrap:break-word; }
    .bp3-tag-input .bp3-tag.bp3-active{
      outline:rgba(19, 124, 189, 0.6) auto 2px;
      outline-offset:0;
      -moz-outline-radius:6px; }
  .bp3-tag-input .bp3-input-ghost{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:20px;
    width:80px; }
    .bp3-tag-input .bp3-input-ghost:disabled, .bp3-tag-input .bp3-input-ghost.bp3-disabled{
      cursor:not-allowed; }
  .bp3-tag-input .bp3-button,
  .bp3-tag-input .bp3-spinner{
    margin:3px;
    margin-left:0; }
  .bp3-tag-input .bp3-button{
    min-height:24px;
    min-width:24px;
    padding:0 7px; }
  .bp3-tag-input.bp3-large{
    height:auto;
    min-height:40px; }
    .bp3-tag-input.bp3-large::before,
    .bp3-tag-input.bp3-large > *{
      margin-right:10px; }
    .bp3-tag-input.bp3-large:empty::before,
    .bp3-tag-input.bp3-large > :last-child{
      margin-right:0; }
    .bp3-tag-input.bp3-large .bp3-tag-input-icon{
      margin-left:5px;
      margin-top:10px; }
    .bp3-tag-input.bp3-large .bp3-input-ghost{
      line-height:30px; }
    .bp3-tag-input.bp3-large .bp3-button{
      min-height:30px;
      min-width:30px;
      padding:5px 10px;
      margin:5px;
      margin-left:0; }
    .bp3-tag-input.bp3-large .bp3-spinner{
      margin:8px;
      margin-left:0; }
  .bp3-tag-input.bp3-active{
    background-color:#ffffff;
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-tag-input .bp3-tag-input-icon, .bp3-tag-input.bp3-dark .bp3-tag-input-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-tag-input .bp3-input-ghost, .bp3-tag-input.bp3-dark .bp3-input-ghost{
    color:#f5f8fa; }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-webkit-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-moz-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost:-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::placeholder{
      color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tag-input.bp3-active, .bp3-tag-input.bp3-dark.bp3-active{
    background-color:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-primary, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-success, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-warning, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-danger, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-input-ghost{
  background:none;
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0; }
  .bp3-input-ghost::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost:focus{
    outline:none !important; }
.bp3-toast{
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin:20px 0 0;
  max-width:500px;
  min-width:300px;
  pointer-events:all;
  position:relative !important; }
  .bp3-toast.bp3-toast-enter, .bp3-toast.bp3-toast-appear{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active, .bp3-toast.bp3-toast-appear-active{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-toast.bp3-toast-enter ~ .bp3-toast, .bp3-toast.bp3-toast-appear ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active ~ .bp3-toast, .bp3-toast.bp3-toast-appear-active ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-toast.bp3-toast-exit{
    opacity:1;
    -webkit-filter:blur(0);
            filter:blur(0); }
  .bp3-toast.bp3-toast-exit-active{
    opacity:0;
    -webkit-filter:blur(10px);
            filter:blur(10px);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:opacity, filter;
    transition-property:opacity, filter, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-toast.bp3-toast-exit ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0); }
  .bp3-toast.bp3-toast-exit-active ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px);
    -webkit-transition-delay:50ms;
            transition-delay:50ms;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-toast .bp3-button-group{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    padding:5px;
    padding-left:0; }
  .bp3-toast > .bp3-icon{
    color:#5c7080;
    margin:12px;
    margin-right:0; }
  .bp3-toast.bp3-dark,
  .bp3-dark .bp3-toast{
    background-color:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-toast.bp3-dark > .bp3-icon,
    .bp3-dark .bp3-toast > .bp3-icon{
      color:#a7b6c2; }
  .bp3-toast[class*="bp3-intent-"] a{
    color:rgba(255, 255, 255, 0.7); }
    .bp3-toast[class*="bp3-intent-"] a:hover{
      color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] > .bp3-icon{
    color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button, .bp3-toast[class*="bp3-intent-"] .bp3-button::before,
  .bp3-toast[class*="bp3-intent-"] .bp3-button .bp3-icon, .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    color:rgba(255, 255, 255, 0.7) !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:focus{
    outline-color:rgba(255, 255, 255, 0.5); }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:hover{
    background-color:rgba(255, 255, 255, 0.15) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    background-color:rgba(255, 255, 255, 0.3) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button::after{
    background:rgba(255, 255, 255, 0.3) !important; }
  .bp3-toast.bp3-intent-primary{
    background-color:#137cbd;
    color:#ffffff; }
  .bp3-toast.bp3-intent-success{
    background-color:#0f9960;
    color:#ffffff; }
  .bp3-toast.bp3-intent-warning{
    background-color:#d9822b;
    color:#ffffff; }
  .bp3-toast.bp3-intent-danger{
    background-color:#db3737;
    color:#ffffff; }

.bp3-toast-message{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  padding:11px;
  word-break:break-word; }

.bp3-toast-container{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box !important;
  display:-ms-flexbox !important;
  display:flex !important;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  left:0;
  overflow:hidden;
  padding:0 20px 20px;
  pointer-events:none;
  right:0;
  z-index:40; }
  .bp3-toast-container.bp3-toast-container-in-portal{
    position:fixed; }
  .bp3-toast-container.bp3-toast-container-inline{
    position:absolute; }
  .bp3-toast-container.bp3-toast-container-top{
    top:0; }
  .bp3-toast-container.bp3-toast-container-bottom{
    bottom:0;
    -webkit-box-orient:vertical;
    -webkit-box-direction:reverse;
        -ms-flex-direction:column-reverse;
            flex-direction:column-reverse;
    top:auto; }
  .bp3-toast-container.bp3-toast-container-left{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start; }
  .bp3-toast-container.bp3-toast-container-right{
    -webkit-box-align:end;
        -ms-flex-align:end;
            align-items:flex-end; }

.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active) ~ .bp3-toast, .bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active) ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-exit-active ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-leave-active ~ .bp3-toast{
  -webkit-transform:translateY(60px);
          transform:translateY(60px); }
.bp3-tooltip{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1); }
  .bp3-tooltip .bp3-popover-arrow{
    height:22px;
    position:absolute;
    width:22px; }
    .bp3-tooltip .bp3-popover-arrow::before{
      height:14px;
      margin:4px;
      width:14px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip{
    margin-bottom:11px;
    margin-top:-11px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
      bottom:-8px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip{
    margin-left:11px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
      left:-8px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip{
    margin-top:11px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
      top:-8px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip{
    margin-left:-11px;
    margin-right:11px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
      right:-8px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-tooltip > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-tooltip > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
    top:-0.22183px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
    right:-0.22183px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
    left:-0.22183px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
    bottom:-0.22183px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-tooltip .bp3-popover-content{
    background:#394b59;
    color:#f5f8fa; }
  .bp3-tooltip .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-tooltip .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-tooltip .bp3-popover-arrow-fill{
    fill:#394b59; }
  .bp3-popover-enter > .bp3-tooltip, .bp3-popover-appear > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8); }
  .bp3-popover-enter-active > .bp3-tooltip, .bp3-popover-appear-active > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-popover-exit > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tooltip .bp3-popover-content{
    padding:10px 12px; }
  .bp3-tooltip.bp3-dark,
  .bp3-dark .bp3-tooltip{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-tooltip .bp3-popover-content{
      background:#e1e8ed;
      color:#394b59; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-fill{
      fill:#e1e8ed; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-content{
    background:#137cbd;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-arrow-fill{
    fill:#137cbd; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-content{
    background:#0f9960;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-arrow-fill{
    fill:#0f9960; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-content{
    background:#d9822b;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-arrow-fill{
    fill:#d9822b; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-content{
    background:#db3737;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-arrow-fill{
    fill:#db3737; }

.bp3-tooltip-indicator{
  border-bottom:dotted 1px;
  cursor:help; }
.bp3-tree .bp3-icon, .bp3-tree .bp3-icon-standard, .bp3-tree .bp3-icon-large{
  color:#5c7080; }
  .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-tree .bp3-icon.bp3-intent-success, .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-tree-node-list{
  list-style:none;
  margin:0;
  padding-left:0; }

.bp3-tree-root{
  background-color:transparent;
  cursor:default;
  padding-left:0;
  position:relative; }

.bp3-tree-node-content-0{
  padding-left:0px; }

.bp3-tree-node-content-1{
  padding-left:23px; }

.bp3-tree-node-content-2{
  padding-left:46px; }

.bp3-tree-node-content-3{
  padding-left:69px; }

.bp3-tree-node-content-4{
  padding-left:92px; }

.bp3-tree-node-content-5{
  padding-left:115px; }

.bp3-tree-node-content-6{
  padding-left:138px; }

.bp3-tree-node-content-7{
  padding-left:161px; }

.bp3-tree-node-content-8{
  padding-left:184px; }

.bp3-tree-node-content-9{
  padding-left:207px; }

.bp3-tree-node-content-10{
  padding-left:230px; }

.bp3-tree-node-content-11{
  padding-left:253px; }

.bp3-tree-node-content-12{
  padding-left:276px; }

.bp3-tree-node-content-13{
  padding-left:299px; }

.bp3-tree-node-content-14{
  padding-left:322px; }

.bp3-tree-node-content-15{
  padding-left:345px; }

.bp3-tree-node-content-16{
  padding-left:368px; }

.bp3-tree-node-content-17{
  padding-left:391px; }

.bp3-tree-node-content-18{
  padding-left:414px; }

.bp3-tree-node-content-19{
  padding-left:437px; }

.bp3-tree-node-content-20{
  padding-left:460px; }

.bp3-tree-node-content{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:30px;
  padding-right:5px;
  width:100%; }
  .bp3-tree-node-content:hover{
    background-color:rgba(191, 204, 214, 0.4); }

.bp3-tree-node-caret,
.bp3-tree-node-caret-none{
  min-width:30px; }

.bp3-tree-node-caret{
  color:#5c7080;
  cursor:pointer;
  padding:7px;
  -webkit-transform:rotate(0deg);
          transform:rotate(0deg);
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tree-node-caret:hover{
    color:#182026; }
  .bp3-dark .bp3-tree-node-caret{
    color:#a7b6c2; }
    .bp3-dark .bp3-tree-node-caret:hover{
      color:#f5f8fa; }
  .bp3-tree-node-caret.bp3-tree-node-caret-open{
    -webkit-transform:rotate(90deg);
            transform:rotate(90deg); }
  .bp3-tree-node-caret.bp3-icon-standard::before{
    content:""; }

.bp3-tree-node-icon{
  margin-right:7px;
  position:relative; }

.bp3-tree-node-label{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-label span{
    display:inline; }

.bp3-tree-node-secondary-label{
  padding:0 5px;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-secondary-label .bp3-popover-wrapper,
  .bp3-tree-node-secondary-label .bp3-popover-target{
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-content{
  background-color:inherit;
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-caret,
.bp3-tree-node.bp3-disabled .bp3-tree-node-icon{
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content,
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-standard, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-large{
    color:#ffffff; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret::before{
    color:rgba(255, 255, 255, 0.7); }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret:hover::before{
    color:#ffffff; }

.bp3-dark .bp3-tree-node-content:hover{
  background-color:rgba(92, 112, 128, 0.3); }

.bp3-dark .bp3-tree .bp3-icon, .bp3-dark .bp3-tree .bp3-icon-standard, .bp3-dark .bp3-tree .bp3-icon-large{
  color:#a7b6c2; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-dark .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
.bp3-omnibar{
  -webkit-filter:blur(0);
          filter:blur(0);
  opacity:1;
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  left:calc(50% - 250px);
  top:20vh;
  width:500px;
  z-index:21; }
  .bp3-omnibar.bp3-overlay-enter, .bp3-omnibar.bp3-overlay-appear{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2; }
  .bp3-omnibar.bp3-overlay-enter-active, .bp3-omnibar.bp3-overlay-appear-active{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-omnibar.bp3-overlay-exit{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1; }
  .bp3-omnibar.bp3-overlay-exit-active{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-omnibar .bp3-input{
    background-color:transparent;
    border-radius:0; }
    .bp3-omnibar .bp3-input, .bp3-omnibar .bp3-input:focus{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-omnibar .bp3-menu{
    background-color:transparent;
    border-radius:0;
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
    max-height:calc(60vh - 40px);
    overflow:auto; }
    .bp3-omnibar .bp3-menu:empty{
      display:none; }
  .bp3-dark .bp3-omnibar, .bp3-omnibar.bp3-dark{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-omnibar-overlay .bp3-overlay-backdrop{
  background-color:rgba(16, 22, 26, 0.2); }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }

.bp3-multi-select{
  min-width:150px; }

.bp3-multi-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto; }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1pY29uLWJyYW5kMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNmZmYiPgogICAgPHBhdGggZD0iTTEwNSAxMjcuM2g0MHYxMi44aC00MHpNNTEuMSA3N0w3NCA5OS45bC0yMy4zIDIzLjMgMTAuNSAxMC41IDIzLjMtMjMuM0w5NSA5OS45IDg0LjUgODkuNCA2MS42IDY2LjV6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNGOUE4MjUiPgogICAgPHBhdGggZD0iTTIwLjIgMTEuOGMtMS42IDAtMS43LjUtMS43IDEgMCAuNC4xLjkuMSAxLjMuMS41LjEuOS4xIDEuMyAwIDEuNy0xLjQgMi4zLTMuNSAyLjNoLS45di0xLjloLjVjMS4xIDAgMS40IDAgMS40LS44IDAtLjMgMC0uNi0uMS0xIDAtLjQtLjEtLjgtLjEtMS4yIDAtMS4zIDAtMS44IDEuMy0yLTEuMy0uMi0xLjMtLjctMS4zLTIgMC0uNC4xLS44LjEtMS4yLjEtLjQuMS0uNy4xLTEgMC0uOC0uNC0uNy0xLjQtLjhoLS41VjQuMWguOWMyLjIgMCAzLjUuNyAzLjUgMi4zIDAgLjQtLjEuOS0uMSAxLjMtLjEuNS0uMS45LS4xIDEuMyAwIC41LjIgMSAxLjcgMXYxLjh6TTEuOCAxMC4xYzEuNiAwIDEuNy0uNSAxLjctMSAwLS40LS4xLS45LS4xLTEuMy0uMS0uNS0uMS0uOS0uMS0xLjMgMC0xLjYgMS40LTIuMyAzLjUtMi4zaC45djEuOWgtLjVjLTEgMC0xLjQgMC0xLjQuOCAwIC4zIDAgLjYuMSAxIDAgLjIuMS42LjEgMSAwIDEuMyAwIDEuOC0xLjMgMkM2IDExLjIgNiAxMS43IDYgMTNjMCAuNC0uMS44LS4xIDEuMi0uMS4zLS4xLjctLjEgMSAwIC44LjMuOCAxLjQuOGguNXYxLjloLS45Yy0yLjEgMC0zLjUtLjYtMy41LTIuMyAwLS40LjEtLjkuMS0xLjMuMS0uNS4xLS45LjEtMS4zIDAtLjUtLjItMS0xLjctMXYtMS45eiIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSIxMy44IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY3g9IjExIiBjeT0iOC4yIiByPSIyLjEiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgPGcgY2xhc3M9ImpwLWljb24td2FybjAiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4=);
  --jp-icon-listings-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MC45NzggNTAuOTc4IiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA1MC45NzggNTAuOTc4OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+Cgk8Zz4KCQk8cGF0aCBzdHlsZT0iZmlsbDojMDEwMDAyOyIgZD0iTTQzLjUyLDcuNDU4QzM4LjcxMSwyLjY0OCwzMi4zMDcsMCwyNS40ODksMEMxOC42NywwLDEyLjI2NiwyLjY0OCw3LjQ1OCw3LjQ1OAoJCQljLTkuOTQzLDkuOTQxLTkuOTQzLDI2LjExOSwwLDM2LjA2MmM0LjgwOSw0LjgwOSwxMS4yMTIsNy40NTYsMTguMDMxLDcuNDU4YzAsMCwwLjAwMSwwLDAuMDAyLDAKCQkJYzYuODE2LDAsMTMuMjIxLTIuNjQ4LDE4LjAyOS03LjQ1OGM0LjgwOS00LjgwOSw3LjQ1Ny0xMS4yMTIsNy40NTctMTguMDNDNTAuOTc3LDE4LjY3LDQ4LjMyOCwxMi4yNjYsNDMuNTIsNy40NTh6CgkJCSBNNDIuMTA2LDQyLjEwNWMtNC40MzIsNC40MzEtMTAuMzMyLDYuODcyLTE2LjYxNSw2Ljg3MmgtMC4wMDJjLTYuMjg1LTAuMDAxLTEyLjE4Ny0yLjQ0MS0xNi42MTctNi44NzIKCQkJYy05LjE2Mi05LjE2My05LjE2Mi0yNC4wNzEsMC0zMy4yMzNDMTMuMzAzLDQuNDQsMTkuMjA0LDIsMjUuNDg5LDJjNi4yODQsMCwxMi4xODYsMi40NCwxNi42MTcsNi44NzIKCQkJYzQuNDMxLDQuNDMxLDYuODcxLDEwLjMzMiw2Ljg3MSwxNi42MTdDNDguOTc3LDMxLjc3Miw0Ni41MzYsMzcuNjc1LDQyLjEwNiw0Mi4xMDV6Ii8+CgkJPHBhdGggc3R5bGU9ImZpbGw6IzAxMDAwMjsiIGQ9Ik0yMy41NzgsMzIuMjE4Yy0wLjAyMy0xLjczNCwwLjE0My0zLjA1OSwwLjQ5Ni0zLjk3MmMwLjM1My0wLjkxMywxLjExLTEuOTk3LDIuMjcyLTMuMjUzCgkJCWMwLjQ2OC0wLjUzNiwwLjkyMy0xLjA2MiwxLjM2Ny0xLjU3NWMwLjYyNi0wLjc1MywxLjEwNC0xLjQ3OCwxLjQzNi0yLjE3NWMwLjMzMS0wLjcwNywwLjQ5NS0xLjU0MSwwLjQ5NS0yLjUKCQkJYzAtMS4wOTYtMC4yNi0yLjA4OC0wLjc3OS0yLjk3OWMtMC41NjUtMC44NzktMS41MDEtMS4zMzYtMi44MDYtMS4zNjljLTEuODAyLDAuMDU3LTIuOTg1LDAuNjY3LTMuNTUsMS44MzIKCQkJYy0wLjMwMSwwLjUzNS0wLjUwMywxLjE0MS0wLjYwNywxLjgxNGMtMC4xMzksMC43MDctMC4yMDcsMS40MzItMC4yMDcsMi4xNzRoLTIuOTM3Yy0wLjA5MS0yLjIwOCwwLjQwNy00LjExNCwxLjQ5My01LjcxOQoJCQljMS4wNjItMS42NCwyLjg1NS0yLjQ4MSw1LjM3OC0yLjUyN2MyLjE2LDAuMDIzLDMuODc0LDAuNjA4LDUuMTQxLDEuNzU4YzEuMjc4LDEuMTYsMS45MjksMi43NjQsMS45NSw0LjgxMQoJCQljMCwxLjE0Mi0wLjEzNywyLjExMS0wLjQxLDIuOTExYy0wLjMwOSwwLjg0NS0wLjczMSwxLjU5My0xLjI2OCwyLjI0M2MtMC40OTIsMC42NS0xLjA2OCwxLjMxOC0xLjczLDIuMDAyCgkJCWMtMC42NSwwLjY5Ny0xLjMxMywxLjQ3OS0xLjk4NywyLjM0NmMtMC4yMzksMC4zNzctMC40MjksMC43NzctMC41NjUsMS4xOTljLTAuMTYsMC45NTktMC4yMTcsMS45NTEtMC4xNzEsMi45NzkKCQkJQzI2LjU4OSwzMi4yMTgsMjMuNTc4LDMyLjIxOCwyMy41NzgsMzIuMjE4eiBNMjMuNTc4LDM4LjIydi0zLjQ4NGgzLjA3NnYzLjQ4NEgyMy41Nzh6Ii8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMEQ0N0ExIj4KICAgIDxwYXRoIGQ9Ik0xMS4xIDYuOVY1LjhINi45YzAtLjUgMC0xLjMuMi0xLjYuNC0uNy44LTEuMSAxLjctMS40IDEuNy0uMyAyLjUtLjMgMy45LS4xIDEgLjEgMS45LjkgMS45IDEuOXY0LjJjMCAuNS0uOSAxLjYtMiAxLjZIOC44Yy0xLjUgMC0yLjQgMS40LTIuNCAyLjh2Mi4ySDQuN0MzLjUgMTUuMSAzIDE0IDMgMTMuMVY5Yy0uMS0xIC42LTIgMS44LTIgMS41LS4xIDYuMy0uMSA2LjMtLjF6Ii8+CiAgICA8cGF0aCBkPSJNMTAuOSAxNS4xdjEuMWg0LjJjMCAuNSAwIDEuMy0uMiAxLjYtLjQuNy0uOCAxLjEtMS43IDEuNC0xLjcuMy0yLjUuMy0zLjkuMS0xLS4xLTEuOS0uOS0xLjktMS45di00LjJjMC0uNS45LTEuNiAyLTEuNmgzLjhjMS41IDAgMi40LTEuNCAyLjQtMi44VjYuNmgxLjdDMTguNSA2LjkgMTkgOCAxOSA4LjlWMTNjMCAxLS43IDIuMS0xLjkgMi4xaC02LjJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4=);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMikiIGZpbGw9IiMzMzMzMzMiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uLWFjY2VudDIganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGQ9Ik01LjA1NjY0IDguNzYxNzJDNS4wNTY2NCA4LjU5NzY2IDUuMDMxMjUgOC40NTMxMiA0Ljk4MDQ3IDguMzI4MTJDNC45MzM1OSA4LjE5OTIyIDQuODU1NDcgOC4wODIwMyA0Ljc0NjA5IDcuOTc2NTZDNC42NDA2MiA3Ljg3MTA5IDQuNSA3Ljc3NTM5IDQuMzI0MjIgNy42ODk0NUM0LjE1MjM0IDcuNTk5NjEgMy45NDMzNiA3LjUxMTcyIDMuNjk3MjcgNy40MjU3OEMzLjMwMjczIDcuMjg1MTYgMi45NDMzNiA3LjEzNjcyIDIuNjE5MTQgNi45ODA0N0MyLjI5NDkyIDYuODI0MjIgMi4wMTc1OCA2LjY0MjU4IDEuNzg3MTEgNi40MzU1NUMxLjU2MDU1IDYuMjI4NTIgMS4zODQ3NyA1Ljk4ODI4IDEuMjU5NzcgNS43MTQ4NEMxLjEzNDc3IDUuNDM3NSAxLjA3MjI3IDUuMTA5MzggMS4wNzIyNyA0LjczMDQ3QzEuMDcyMjcgNC4zOTg0NCAxLjEyODkxIDQuMDk1NyAxLjI0MjE5IDMuODIyMjdDMS4zNTU0NyAzLjU0NDkyIDEuNTE1NjIgMy4zMDQ2OSAxLjcyMjY2IDMuMTAxNTZDMS45Mjk2OSAyLjg5ODQ0IDIuMTc5NjkgMi43MzQzNyAyLjQ3MjY2IDIuNjA5MzhDMi43NjU2MiAyLjQ4NDM4IDMuMDkxOCAyLjQwNDMgMy40NTExNyAyLjM2OTE0VjEuMTA5MzhINC4zODg2N1YyLjM4MDg2QzQuNzQwMjMgMi40Mjc3MyA1LjA1NjY0IDIuNTIzNDQgNS4zMzc4OSAyLjY2Nzk3QzUuNjE5MTQgMi44MTI1IDUuODU3NDIgMy4wMDE5NSA2LjA1MjczIDMuMjM2MzNDNi4yNTE5NSAzLjQ2NjggNi40MDQzIDMuNzQwMjMgNi41MDk3NyA0LjA1NjY0QzYuNjE5MTQgNC4zNjkxNCA2LjY3MzgzIDQuNzIwNyA2LjY3MzgzIDUuMTExMzNINS4wNDQ5MkM1LjA0NDkyIDQuNjM4NjcgNC45Mzc1IDQuMjgxMjUgNC43MjI2NiA0LjAzOTA2QzQuNTA3ODEgMy43OTI5NyA0LjIxNjggMy42Njk5MiAzLjg0OTYxIDMuNjY5OTJDMy42NTAzOSAzLjY2OTkyIDMuNDc2NTYgMy42OTcyNyAzLjMyODEyIDMuNzUxOTVDMy4xODM1OSAzLjgwMjczIDMuMDY0NDUgMy44NzY5NSAyLjk3MDcgMy45NzQ2MUMyLjg3Njk1IDQuMDY4MzYgMi44MDY2NCA0LjE3OTY5IDIuNzU5NzcgNC4zMDg1OUMyLjcxNjggNC40Mzc1IDIuNjk1MzEgNC41NzgxMiAyLjY5NTMxIDQuNzMwNDdDMi42OTUzMSA0Ljg4MjgxIDIuNzE2OCA1LjAxOTUzIDIuNzU5NzcgNS4xNDA2MkMyLjgwNjY0IDUuMjU3ODEgMi44ODI4MSA1LjM2NzE5IDIuOTg4MjggNS40Njg3NUMzLjA5NzY2IDUuNTcwMzEgMy4yNDAyMyA1LjY2Nzk3IDMuNDE2MDIgNS43NjE3MkMzLjU5MTggNS44NTE1NiAzLjgxMDU1IDUuOTQzMzYgNC4wNzIyNyA2LjAzNzExQzQuNDY2OCA2LjE4NTU1IDQuODI0MjIgNi4zMzk4NCA1LjE0NDUzIDYuNUM1LjQ2NDg0IDYuNjU2MjUgNS43MzgyOCA2LjgzOTg0IDUuOTY0ODQgNy4wNTA3OEM2LjE5NTMxIDcuMjU3ODEgNi4zNzEwOSA3LjUgNi40OTIxOSA3Ljc3NzM0QzYuNjE3MTkgOC4wNTA3OCA2LjY3OTY5IDguMzc1IDYuNjc5NjkgOC43NUM2LjY3OTY5IDkuMDkzNzUgNi42MjMwNSA5LjQwNDMgNi41MDk3NyA5LjY4MTY0QzYuMzk2NDggOS45NTUwOCA2LjIzNDM4IDEwLjE5MTQgNi4wMjM0NCAxMC4zOTA2QzUuODEyNSAxMC41ODk4IDUuNTU4NTkgMTAuNzUgNS4yNjE3MiAxMC44NzExQzQuOTY0ODQgMTAuOTg4MyA0LjYzMjgxIDExLjA2NDUgNC4yNjU2MiAxMS4wOTk2VjEyLjI0OEgzLjMzMzk4VjExLjA5OTZDMy4wMDE5NSAxMS4wNjg0IDIuNjc5NjkgMTAuOTk2MSAyLjM2NzE5IDEwLjg4MjhDMi4wNTQ2OSAxMC43NjU2IDEuNzc3MzQgMTAuNTk3NyAxLjUzNTE2IDEwLjM3ODlDMS4yOTY4OCAxMC4xNjAyIDEuMTA1NDcgOS44ODQ3NyAwLjk2MDkzOCA5LjU1MjczQzAuODE2NDA2IDkuMjE2OCAwLjc0NDE0MSA4LjgxNDQ1IDAuNzQ0MTQxIDguMzQ1N0gyLjM3ODkxQzIuMzc4OTEgOC42MjY5NSAyLjQxOTkyIDguODYzMjggMi41MDE5NSA5LjA1NDY5QzIuNTgzOTggOS4yNDIxOSAyLjY4OTQ1IDkuMzkyNTggMi44MTgzNiA5LjUwNTg2QzIuOTUxMTcgOS42MTUyMyAzLjEwMTU2IDkuNjkzMzYgMy4yNjk1MyA5Ljc0MDIzQzMuNDM3NSA5Ljc4NzExIDMuNjA5MzggOS44MTA1NSAzLjc4NTE2IDkuODEwNTVDNC4yMDMxMiA5LjgxMDU1IDQuNTE5NTMgOS43MTI4OSA0LjczNDM4IDkuNTE3NThDNC45NDkyMiA5LjMyMjI3IDUuMDU2NjQgOS4wNzAzMSA1LjA1NjY0IDguNzYxNzJaTTEzLjQxOCAxMi4yNzE1SDguMDc0MjJWMTFIMTMuNDE4VjEyLjI3MTVaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzLjk1MjY0IDYpIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTUgMTVIM3YyaDEydi0yem0wLThIM3YyaDEyVjd6TTMgMTNoMTh2LTJIM3Yyem0wIDhoMTh2LTJIM3Yyek0zIDN2MmgxOFYzSDN6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4=);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}
.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}
.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}
.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}
.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}
.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}
.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}
.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}
.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}
.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}
.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}
.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}
.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}
.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}
.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}
.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}
.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}
.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}
.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}
.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}
.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}
.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}
.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}
.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}
.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}
.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}
.jp-FileIcon {
  background-image: var(--jp-icon-file);
}
.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}
.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}
.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}
.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}
.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}
.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}
.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}
.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
}
.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}
.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}
.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}
.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}
.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}
.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}
.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}
.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}
.jp-ListIcon {
  background-image: var(--jp-icon-list);
}
.jp-ListingsInfoIcon {
  background-image: var(--jp-icon-listings-info);
}
.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}
.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}
.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}
.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}
.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}
.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}
.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}
.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}
.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
}
.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}
.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}
.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}
.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
}
.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}
.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}
.jp-RunIcon {
  background-image: var(--jp-icon-run);
}
.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}
.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}
.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}
.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}
.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}
.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}
.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}
.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}
.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}
.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}
.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}
.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}
.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}
.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}
.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}
.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}
.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}
/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}
/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}
/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}
.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}
.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}
.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}
.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}
.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}
.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}
.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}
.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}
/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}
.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}
.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}
.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}
.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}
.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}
.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}
/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

/* CSS for icons in selected items in the settings editor */
#setting-editor .jp-PluginList .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
#setting-editor
  .jp-PluginList
  .jp-mod-selected
  .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected tabs in the sidebar tab manager */
#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable[fill] {
  fill: #fff;
}

#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable[fill] {
  fill: var(--jp-brand-color1);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable-inverse[fill] {
  fill: #fff;
}

/**
 * TODO: come up with non css-hack solution for showing the busy icon on top
 *  of the close icon
 * CSS for complex behavior of close icon of tabs in the sidebar tab manager
 */
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-dirty.jp-mod-active
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: #fff;
}

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) svg {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-border-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0px;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-warn-color0);
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

/* Override Blueprint's _reset.scss styles */
html {
  box-sizing: unset;
}

*,
*::before,
*::after {
  box-sizing: unset;
}

body {
  color: unset;
  font-family: var(--jp-ui-font-family);
}

p {
  margin-top: unset;
  margin-bottom: unset;
}

small {
  font-size: unset;
}

strong {
  font-weight: unset;
}

/* Override Blueprint's _typography.scss styles */
a {
  text-decoration: unset;
  color: unset;
}
a:hover {
  text-decoration: unset;
  color: unset;
}

/* Override Blueprint's _accessibility.scss styles */
:focus {
  outline: unset;
  outline-offset: unset;
  -moz-outline-radius: unset;
}

/* Styles for ui-components */
.jp-Button {
  border-radius: var(--jp-border-radius);
  padding: 0px 12px;
  font-size: var(--jp-ui-font-size1);
}

/* Use our own theme for hover styles */
button.jp-Button.bp3-button.bp3-minimal:hover {
  background-color: var(--jp-layout-color2);
}
.jp-Button.minimal {
  color: unset !important;
}

.jp-Button.jp-ToolbarButtonComponent {
  text-transform: none;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color3);
}

.jp-BPIcon {
  display: inline-block;
  vertical-align: middle;
  margin: auto;
}

/* Stop blueprint futzing with our icon fills */
.bp3-icon.jp-BPIcon > svg:not([fill]) {
  fill: var(--jp-inverse-layout-color3);
}

.jp-InputGroupAction {
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

/* Use our own theme for hover and option styles */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}
select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-top: 1px solid var(--jp-border-color2);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-Collapse-header {
  padding: 1px 12px;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size2);
}

.jp-Collapse-header:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Collapse-contents {
  padding: 0px 12px 0px 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0px;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0px 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px 5px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0px;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty:after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0px 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0px;
  left: 0px;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px;
  padding-bottom: 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
  resize: both;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0px;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0px 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

.jp-HoverBox.jp-mod-outofview {
  display: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;

  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;

  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #aa00ff;

  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;

  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;

  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;

  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;

  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;

  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;

  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;

  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;

  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;

  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ffff00;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;

  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;

  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;

  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;

  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;

  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eeeeee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;

  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent:before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent:after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0px 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FileDialog-Checkbox {
  margin-top: 35px;
  display: flex;
  flex-direction: row;
  align-items: end;
  width: 100%;
}

.jp-FileDialog-Checkbox > label {
  flex: 1 1 auto;
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  height: 28px;
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  background-color: var(--jp-layout-color1);
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0px 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  height: 32px;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 1;
  overflow-x: auto;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px;
  margin: 0px;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px 6px;
  margin: 0px;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent span {
  padding: 0px;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ body.p-mod-override-cursor *, /* </DEPRECATED> */
body.lm-mod-override-cursor * {
  cursor: inherit !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/* BASICS */

.CodeMirror {
  /* Set height, width, borders, and global font properties here */
  font-family: monospace;
  height: 300px;
  color: black;
  direction: ltr;
}

/* PADDING */

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  background-color: white; /* The little square between H and V scrollbars */
}

/* GUTTER */

.CodeMirror-gutters {
  border-right: 1px solid #ddd;
  background-color: #f7f7f7;
  white-space: nowrap;
}
.CodeMirror-linenumbers {}
.CodeMirror-linenumber {
  padding: 0 3px 0 5px;
  min-width: 20px;
  text-align: right;
  color: #999;
  white-space: nowrap;
}

.CodeMirror-guttermarker { color: black; }
.CodeMirror-guttermarker-subtle { color: #999; }

/* CURSOR */

.CodeMirror-cursor {
  border-left: 1px solid black;
  border-right: none;
  width: 0;
}
/* Shown when moving in bi-directional text */
.CodeMirror div.CodeMirror-secondarycursor {
  border-left: 1px solid silver;
}
.cm-fat-cursor .CodeMirror-cursor {
  width: auto;
  border: 0 !important;
  background: #7e7;
}
.cm-fat-cursor div.CodeMirror-cursors {
  z-index: 1;
}
.cm-fat-cursor-mark {
  background-color: rgba(20, 255, 20, 0.5);
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
}
.cm-animate-fat-cursor {
  width: auto;
  border: 0;
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
  background-color: #7e7;
}
@-moz-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@-webkit-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}

/* Can style cursor different in overwrite (non-insert) mode */
.CodeMirror-overwrite .CodeMirror-cursor {}

.cm-tab { display: inline-block; text-decoration: inherit; }

.CodeMirror-rulers {
  position: absolute;
  left: 0; right: 0; top: -50px; bottom: 0;
  overflow: hidden;
}
.CodeMirror-ruler {
  border-left: 1px solid #ccc;
  top: 0; bottom: 0;
  position: absolute;
}

/* DEFAULT THEME */

.cm-s-default .cm-header {color: blue;}
.cm-s-default .cm-quote {color: #090;}
.cm-negative {color: #d44;}
.cm-positive {color: #292;}
.cm-header, .cm-strong {font-weight: bold;}
.cm-em {font-style: italic;}
.cm-link {text-decoration: underline;}
.cm-strikethrough {text-decoration: line-through;}

.cm-s-default .cm-keyword {color: #708;}
.cm-s-default .cm-atom {color: #219;}
.cm-s-default .cm-number {color: #164;}
.cm-s-default .cm-def {color: #00f;}
.cm-s-default .cm-variable,
.cm-s-default .cm-punctuation,
.cm-s-default .cm-property,
.cm-s-default .cm-operator {}
.cm-s-default .cm-variable-2 {color: #05a;}
.cm-s-default .cm-variable-3, .cm-s-default .cm-type {color: #085;}
.cm-s-default .cm-comment {color: #a50;}
.cm-s-default .cm-string {color: #a11;}
.cm-s-default .cm-string-2 {color: #f50;}
.cm-s-default .cm-meta {color: #555;}
.cm-s-default .cm-qualifier {color: #555;}
.cm-s-default .cm-builtin {color: #30a;}
.cm-s-default .cm-bracket {color: #997;}
.cm-s-default .cm-tag {color: #170;}
.cm-s-default .cm-attribute {color: #00c;}
.cm-s-default .cm-hr {color: #999;}
.cm-s-default .cm-link {color: #00c;}

.cm-s-default .cm-error {color: #f00;}
.cm-invalidchar {color: #f00;}

.CodeMirror-composing { border-bottom: 2px solid; }

/* Default styles for common addons */

div.CodeMirror span.CodeMirror-matchingbracket {color: #0b0;}
div.CodeMirror span.CodeMirror-nonmatchingbracket {color: #a22;}
.CodeMirror-matchingtag { background: rgba(255, 150, 0, .3); }
.CodeMirror-activeline-background {background: #e8f2ff;}

/* STOP */

/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: white;
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px; margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}
.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}
.CodeMirror-vscrollbar {
  right: 0; top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}
.CodeMirror-hscrollbar {
  bottom: 0; left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}
.CodeMirror-scrollbar-filler {
  right: 0; bottom: 0;
}
.CodeMirror-gutter-filler {
  left: 0; bottom: 0;
}

.CodeMirror-gutters {
  position: absolute; left: 0; top: 0;
  min-height: 100%;
  z-index: 3;
}
.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}
.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}
.CodeMirror-gutter-background {
  position: absolute;
  top: 0; bottom: 0;
  z-index: 4;
}
.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}
.CodeMirror-gutter-wrapper ::selection { background-color: transparent }
.CodeMirror-gutter-wrapper ::-moz-selection { background-color: transparent }

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  -moz-border-radius: 0; -webkit-border-radius: 0; border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}
.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0; right: 0; top: 0; bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-widget {}

.CodeMirror-rtl pre { direction: rtl; }

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}
.CodeMirror-measure pre { position: static; }

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}
div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected { background: #d9d9d9; }
.CodeMirror-focused .CodeMirror-selected { background: #d7d4f0; }
.CodeMirror-crosshair { cursor: crosshair; }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: #d7d4f0; }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: #d7d4f0; }

.cm-searching {
  background-color: #ffa;
  background-color: rgba(255, 255, 0, .4);
}

/* Used to force a border model for a node */
.cm-force-border { padding-right: .1px; }

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack:after { content: ''; }

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext { background: none; }

.CodeMirror-dialog {
  position: absolute;
  left: 0; right: 0;
  background: inherit;
  z-index: 15;
  padding: .1em .8em;
  overflow: hidden;
  color: inherit;
}

.CodeMirror-dialog-top {
  border-bottom: 1px solid #eee;
  top: 0;
}

.CodeMirror-dialog-bottom {
  border-top: 1px solid #eee;
  bottom: 0;
}

.CodeMirror-dialog input {
  border: none;
  outline: none;
  background: transparent;
  width: 20em;
  color: inherit;
  font-family: monospace;
}

.CodeMirror-dialog button {
  font-size: 70%;
}

.CodeMirror-foldmarker {
  color: blue;
  text-shadow: #b9f 1px 1px 2px, #b9f -1px -1px 2px, #b9f 1px -1px 2px, #b9f -1px 1px 2px;
  font-family: arial;
  line-height: .3;
  cursor: pointer;
}
.CodeMirror-foldgutter {
  width: .7em;
}
.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
}
.CodeMirror-foldgutter-open:after {
  content: "\25BE";
}
.CodeMirror-foldgutter-folded:after {
  content: "\25B8";
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.CodeMirror {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;
  /* Changed to auto to autogrow */
}

.CodeMirror pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* This causes https://github.com/jupyter/jupyterlab/issues/522 */
/* May not cause it not because we changed it! */
.CodeMirror-lines {
  padding: var(--jp-code-padding) 0;
}

.CodeMirror-linenumber {
  padding: 0 8px;
}

.jp-CodeMirrorEditor {
  cursor: text;
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.CodeMirror.jp-mod-readOnly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--jp-border-color2);
  background-color: var(--jp-layout-color0);
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.CodeMirror-selectedtext.cm-searching {
  background-color: var(--jp-search-selected-match-background-color) !important;
  color: var(--jp-search-selected-match-color) !important;
}

.cm-searching {
  background-color: var(
    --jp-search-unselected-match-background-color
  ) !important;
  color: var(--jp-search-unselected-match-color) !important;
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--jp-editor-selected-focused-background);
}

.CodeMirror-selected {
  background-color: var(--jp-editor-selected-background);
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/**
 * Here is our jupyter theme for CodeMirror syntax highlighting
 * This is used in our marked.js syntax highlighting and CodeMirror itself
 * The string "jupyter" is set in ../codemirror/widget.DEFAULT_CODEMIRROR_THEME
 * This came from the classic notebook, which came form highlight.js/GitHub
 */

/**
 * CodeMirror themes are handling the background/color in this way. This works
 * fine for CodeMirror editors outside the notebook, but the notebook styles
 * these things differently.
 */
.CodeMirror.cm-s-jupyter {
  background: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* In the notebook, we want this styling to be handled by its container */
.jp-CodeConsole .CodeMirror.cm-s-jupyter,
.jp-Notebook .CodeMirror.cm-s-jupyter {
  background: transparent;
}

.cm-s-jupyter .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}
.cm-s-jupyter span.cm-keyword {
  color: var(--jp-mirror-editor-keyword-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-atom {
  color: var(--jp-mirror-editor-atom-color);
}
.cm-s-jupyter span.cm-number {
  color: var(--jp-mirror-editor-number-color);
}
.cm-s-jupyter span.cm-def {
  color: var(--jp-mirror-editor-def-color);
}
.cm-s-jupyter span.cm-variable {
  color: var(--jp-mirror-editor-variable-color);
}
.cm-s-jupyter span.cm-variable-2 {
  color: var(--jp-mirror-editor-variable-2-color);
}
.cm-s-jupyter span.cm-variable-3 {
  color: var(--jp-mirror-editor-variable-3-color);
}
.cm-s-jupyter span.cm-punctuation {
  color: var(--jp-mirror-editor-punctuation-color);
}
.cm-s-jupyter span.cm-property {
  color: var(--jp-mirror-editor-property-color);
}
.cm-s-jupyter span.cm-operator {
  color: var(--jp-mirror-editor-operator-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-comment {
  color: var(--jp-mirror-editor-comment-color);
  font-style: italic;
}
.cm-s-jupyter span.cm-string {
  color: var(--jp-mirror-editor-string-color);
}
.cm-s-jupyter span.cm-string-2 {
  color: var(--jp-mirror-editor-string-2-color);
}
.cm-s-jupyter span.cm-meta {
  color: var(--jp-mirror-editor-meta-color);
}
.cm-s-jupyter span.cm-qualifier {
  color: var(--jp-mirror-editor-qualifier-color);
}
.cm-s-jupyter span.cm-builtin {
  color: var(--jp-mirror-editor-builtin-color);
}
.cm-s-jupyter span.cm-bracket {
  color: var(--jp-mirror-editor-bracket-color);
}
.cm-s-jupyter span.cm-tag {
  color: var(--jp-mirror-editor-tag-color);
}
.cm-s-jupyter span.cm-attribute {
  color: var(--jp-mirror-editor-attribute-color);
}
.cm-s-jupyter span.cm-header {
  color: var(--jp-mirror-editor-header-color);
}
.cm-s-jupyter span.cm-quote {
  color: var(--jp-mirror-editor-quote-color);
}
.cm-s-jupyter span.cm-link {
  color: var(--jp-mirror-editor-link-color);
}
.cm-s-jupyter span.cm-error {
  color: var(--jp-mirror-editor-error-color);
}
.cm-s-jupyter span.cm-hr {
  color: #999;
}

.cm-s-jupyter span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}

.cm-s-jupyter .CodeMirror-activeline-background,
.cm-s-jupyter .CodeMirror-gutter {
  background-color: var(--jp-layout-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .remote-caret {
  position: relative;
  border-left: 2px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .remote-caret > div {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -2px;
  font-size: 0.95em;
  background-color: rgb(250, 129, 0);
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 3;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .remote-caret.hide-name > div {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .remote-caret:hover > div {
  opacity: 1;
  transition-delay: 0s;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0px;
  padding: 0px;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}
.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}
.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}
.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}
.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}
.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}
.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}
.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}
.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}
.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}
.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}
.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}
.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}
.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}
.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}
.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}
.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0em;
}

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: 12px;
  table-layout: fixed;
  margin-left: auto;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon table {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0px;
}

.jp-RenderedHTMLCommon p {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}
/* ...or leave it untouched if they don't */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-dark-background {
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-light-background {
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}
.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}
.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}
.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}
.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}
.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}
.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}
.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}
.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: 0.8em;
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser {
  display: flex;
  flex-direction: column;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  border-bottom: none;
  height: auto;
  margin: var(--jp-toolbar-header-margin);
  box-shadow: none;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0px 2px;
  padding: 0px 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0px;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar.jp-Toolbar {
  padding: 0px;
  margin: 8px 12px 0px 12px;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  justify-content: flex-start;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0px;
  padding-right: 2px;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-ToolbarButtonComponent {
  width: 40px;
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent {
  width: 72px;
  background: var(--jp-brand-color1);
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent:focus-visible {
  background-color: var(--jp-brand-color0);
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent
  .jp-icon3 {
  fill: white;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileBrowser-filterBox {
  padding: 0px;
  flex: 0 0 auto;
  margin: 8px 12px 0px 12px;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing:focus-visible {
  border: 1px solid var(--jp-brand-color1);
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px 12px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon:before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon:before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0px;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-DirListing-deadSpace {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
}

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: flex;
  flex-direction: row;
}

body[data-format='mobile'] .jp-OutputArea-child {
  flex-direction: column;
}

.jp-OutputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);
  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

body[data-format='mobile'] .jp-OutputPrompt {
  flex: 0 0 auto;
  text-align: left;
}

.jp-OutputArea-output {
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea-child .jp-OutputArea-output {
  flex-grow: 1;
  flex-shrink: 1;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
  margin-left: var(--jp-notebook-padding);
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0px;
  padding: 0px;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0px;
  flex: 1 1 auto;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-OutputArea-stdin {
  line-height: var(--jp-code-line-height);
  padding-top: var(--jp-code-padding);
  display: flex;
}

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0px;
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;
  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0px;
  bottom: 0px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0px;
  width: 100%;
  padding: 0px;
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: flex;
  flex-direction: row;
  overflow: hidden;
}

body[data-format='mobile'] .jp-InputArea {
  flex-direction: column;
}

.jp-InputArea-editor {
  flex: 1 1 auto;
  overflow: hidden;
}

.jp-InputArea-editor {
  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0px;
  background: var(--jp-cell-editor-background);
}

body[data-format='mobile'] .jp-InputArea-editor {
  margin-left: var(--jp-notebook-padding);
}

.jp-InputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);
  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

body[data-format='mobile'] .jp-InputPrompt {
  flex: 0 0 auto;
  text-align: left;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: flex;
  flex-direction: row;
  flex: 1 1 auto;
}

.jp-Placeholder-prompt {
  box-sizing: border-box;
}

.jp-Placeholder-content {
  flex: 1 1 auto;
  border: none;
  background: transparent;
  height: 20px;
  box-sizing: border-box;
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0px;
  margin: 0px;
  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 200px;
  box-shadow: inset 0 0 6px 2px rgba(0, 0, 0, 0.3);
  margin-left: var(--jp-private-cell-scrolling-output-offset);
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  flex: 0 0
    calc(
      var(--jp-cell-prompt-width) -
        var(--jp-private-cell-scrolling-output-offset)
    );
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  flex: 1 1 auto;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

.jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
}

.jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-collapseHeadingButton {
  display: none;
}

.jp-MarkdownCell:hover .jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: 2px;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
}

.jp-Notebook-render * {
  contain: none !important;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
  float: left;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt:before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0px;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-NotebookTools-tool {
  padding: 0px 12px 0 12px;
}

.jp-ActiveCellTool {
  padding: 12px;
  background-color: var(--jp-layout-color1);
  border-top: none !important;
}

.jp-ActiveCellTool .jp-InputArea-prompt {
  flex: 0 0 auto;
  padding-left: 0px;
}

.jp-ActiveCellTool .jp-InputArea-editor {
  flex: 1 1 auto;
  background: var(--jp-cell-editor-background);
  border-color: var(--jp-cell-editor-border-color);
}

.jp-ActiveCellTool .jp-InputArea-editor .CodeMirror {
  background: transparent;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0px 12px 0px;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body div {
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

</style>

    <style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
    0px 1px 3px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
    0px 1px 5px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
    0px 1px 10px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
    0px 1px 18px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
    0px 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
    0px 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
    0px 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
    0px 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
    0px 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;

  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;

  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);

  --jp-content-link-color: var(--md-blue-700);

  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);

  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);

  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);

  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);

  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;

  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;

  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);

  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0px;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;
  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0px 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-border-color1);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: #05a;
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #aa22ff;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #aa22ff;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);
}
</style>

<style type="text/css">
/* Misc */
a.anchor-link {
  display: none;
}

.highlight  {
  margin: 0.4em;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

/* Using table instead of flexbox so that we can use break-inside property */
/* CSS rules under this comment should not be required anymore after we move to the JupyterLab 4.0 CSS */


.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  min-width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-OutputArea-child {
  display: table;
  width: 100%;
}

.jp-OutputPrompt {
  display: table-cell;
  vertical-align: top;
  min-width: var(--jp-cell-prompt-width);
}

body[data-format='mobile'] .jp-OutputPrompt {
  display: table-row;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
  display: table-row;
}

.jp-OutputArea-output.jp-OutputArea-executeResult {
  width: 100%;
}

@media print {
  .jp-Collapser {
    display: none;
  }

  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }

  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}
</style>

<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                CommonHTML: {
                    linebreaks: { 
                    automatic: true 
                    }
                }
            });
        
            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
    <!-- End of mathjax configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">

<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Welcome somthing intro.</p>
<p>For some background, every patch of World of Warcraft releases a new raid tier and season. Each expansion contains a range of dungeons that 5 people will go in and attempt to complete. There have been varying difficulties over the years, but more recently, it has been toned to normal, heroic, and mythic difficulties, with mythic containing a trial mode based on an affix and key system. Each dungeon group contains a tank, a healer, and 3 damage dealers. The focus of this document is to analyze damage dealer class performance and representation, and possible attempt to identify which types of classes have a history of success to determine which class to play going into the new expansion: Dragonflight.</p>
<p>Goals: h0: melee vs range difference = 0 across an entire raid</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Imports for project</span>
<span class="kn">import</span> <span class="nn">requests</span>
<span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span> <span class="k">as</span> <span class="n">bs</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span>
<span class="kn">from</span> <span class="nn">sklearn</span> <span class="kn">import</span> <span class="n">linear_model</span>

<span class="c1">#Set figure size</span>
<span class="n">sns</span><span class="o">.</span><span class="n">set</span><span class="p">(</span><span class="n">rc</span> <span class="o">=</span> <span class="p">{</span><span class="s1">&#39;figure.figsize&#39;</span><span class="p">:(</span><span class="mi">18</span><span class="p">,</span><span class="mi">8</span><span class="p">)})</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>To start, let's look at the most recent season in the 9.2 patch. To do so, we have to pull data from the warcraft API, and using raider.io to confirm the information. Raider.io also pulls from the warcraft api to compile comprehensive leader boards for raid and dungeon rankings.</p>
<p>From raider.io we can pull each classes' spec performers over the 9.2 mythic dungeon season patch. The Score associated with each player is calculated based on the highest level completion (with a bonus to competions within the time limit) across all dungeons in the expansion. Each dungeon carries a high score, and the total player score value is aggregated across all available dungeons. In short, a higher score means higher average difficulty dungeon competions.</p>
<p>To expand a bit more on the key system, after a dungeon is completed, a key to a random dungeon is dropped for all members. This key increases the difficulty of the next dungeon, scaling infinitely. Rewards are capped at +15, but the score reward is uncapped. Groups will try to push higher keys in an attempt to gain more score for the leaderboards.</p>
<p>The data stored within the following table contains the top 10 players for each dps specialization for each class.</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Dungeon92Ranks</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="s1">&#39;WowDungeon9.2Rankings.csv&#39;</span><span class="p">)</span>
<span class="n">Dungeon92Ranks</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[2]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Class</th>
      <th>Spec</th>
      <th>Rank</th>
      <th>Covenant</th>
      <th>Score</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Death Knight</td>
      <td>Frost DK</td>
      <td>1</td>
      <td>Nightfae</td>
      <td>3672.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Death Knight</td>
      <td>Frost DK</td>
      <td>2</td>
      <td>Nightfae</td>
      <td>3590.3</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Death Knight</td>
      <td>Frost DK</td>
      <td>3</td>
      <td>Kyrian</td>
      <td>3557.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Death Knight</td>
      <td>Frost DK</td>
      <td>4</td>
      <td>Nightfae</td>
      <td>3554.3</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Death Knight</td>
      <td>Frost DK</td>
      <td>5</td>
      <td>Nightfae</td>
      <td>3548.8</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>235</th>
      <td>Warrior</td>
      <td>Fury</td>
      <td>6</td>
      <td>Nightfae</td>
      <td>3670.0</td>
    </tr>
    <tr>
      <th>236</th>
      <td>Warrior</td>
      <td>Fury</td>
      <td>7</td>
      <td>Kyrian</td>
      <td>3634.0</td>
    </tr>
    <tr>
      <th>237</th>
      <td>Warrior</td>
      <td>Fury</td>
      <td>8</td>
      <td>Kyrian</td>
      <td>3622.5</td>
    </tr>
    <tr>
      <th>238</th>
      <td>Warrior</td>
      <td>Fury</td>
      <td>9</td>
      <td>Kyrian</td>
      <td>3610.6</td>
    </tr>
    <tr>
      <th>239</th>
      <td>Warrior</td>
      <td>Fury</td>
      <td>10</td>
      <td>Necrolord</td>
      <td>3585.0</td>
    </tr>
  </tbody>
</table>
<p>240 rows × 5 columns</p>
</div>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>For a surface level analysis, let's plot the average score by class.</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Class&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Score&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">Dungeon92Ranks</span><span class="p">)</span><span class="c1">#, height= 7, fit_reg=False) </span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">(</span><span class="n">rotation</span><span class="o">=</span><span class="mi">45</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">&#39;seaborn-white&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;IO Score by Class&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Class&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Score&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">(</span><span class="mi">3000</span><span class="p">,</span> <span class="mi">4000</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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N99UcnKyvv76a+vaEufPn1fv3r1lNpsfue2tW7dUsGBBubi46OrVq9q1a5diYmIkSZ06ddK5c+ckSUWLFrWeNvK4/QAA4N9xWVMAADK5PHnyaO7cuRo/frwmT54sOzs7eXt7a+LEiSpfvvzfbv/SSy8pICBAQ4YM0d27d5WcnKycOXNqwoQJyp07t3Lnzq127drp7bfflqOjo6pWrao33nhDJpNJHTt2VKtWrZScnKwSJUpoyJAh/5ipVatWunr1qho3biyLxaLSpUvr448//sfb1qxZU5999pmuXLmi0qVL691337X+rHHjxpo0aZJq1679j/c1m82aP3++xowZowYNGihLlixyd3dXv379/nYKyfvvv6/PPvtMtWrVUunSpdWvXz917dpV8+bNU+vWrdWzZ08lJCRIkj744APlz5//sfsBAMC/M1n+OgcSAAAgg9i4caO2bNmiSZMm2ToKAAB4SsxJBAAAGVJsbKxmz56tDz/80NZRAADAM3iuhcWIESOsBw0rV65Us2bN9P7772vIkCFKTk6W9OcCX82bN9cHH3ygzz//XHFxcZKkY8eO6f3331erVq3Uvn173b59+3lGBwAA6UhQUJAaNmyomjVrqmLFiraOAwAAnsFzOyXk559/1sSJE2VnZ6cxY8bovffe0/r16+Xu7q4uXbqoYcOGqlevnmrWrKmVK1cqd+7cGj58uDw9PdWpUyc1bNhQX3/9tcqXL6958+YpNDRUAQEBzyM6AAAAAAB4zp7LDIt79+5pzJgx6tu3ryRp3759evXVV63XYq9fv76Cg4N19OhRFSxYULlz55YkNWjQQMHBwbpy5YpiY2OtC381bNhQwcHBzyM6AAAAAACwgedSWAQGBuqTTz5Rjhw5JEk3btyQt7e39edeXl66ceNGivd7enrq5s2bzyM6AAAAAACwgTQvLPbu3avIyEg1atTosbexWCwymUz/eT8AAAAAAMgY7NP6ATZt2qRLly7pvffeU3x8vC5fvqyQkBA1adLEepvw8HD5+vrKz89P4eHhKdrv4+PzVDkiImKUnMwVXAEAAAAAMAo7O5OyZ3f5x5+leWExfPhw65+vXLmifv36afz48Xr33XcVERGhbNmyad26dWrZsqXKlCmjsLAwXb58Wfny5dPatWtVq1Yt+fn5ycPDQyEhIXrllVes+59GcrKFwgIAAAAA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ypX66KOPNGzYMI0ePVqFCxdWrly5bJTW2B4uK65du6bbt2/Lz89PYWFh1lM77ezsdP78eUVERMjb21teXl62jGxYycnJsre31wcffKBr165p9OjRCgkJUbt27RQXF6dp06ZJksLDwxUdHW3o406uEpIO3L59W3fv3lX+/PkVFRWl7t27q3///ipatKhOnDihuXPnKmfOnBowYIAmT56sGjVqqEyZMraOne6cOXNG9vb2yps3r9auXauQkBA1aNBAtWvX1tmzZ5WcnCwPD49Mc8B+8OBBRUZGqkaNGrK3t9fy5cs1fPhwrVixQtmyZdOyZcvUpk0beXp62jqq4T14A7ZYLLp//7569uypHTt2aN68eXrttdcUHBysAQMG6KWXXtKVK1c0duxYFSpUyNaxDefBOIaFhSlHjhxycXHRggULtGXLFg0cOFAlSpTQ/v37FRISogsXLqhFixaGOw/TiNavX6+ff/5ZefLk0VtvvaXjx4/rs88+05w5c/T666/r3r17slgsLLL5lCwWi+7du6eBAwfq3XffVeXKlRUWFqalS5fq4sWL6tatmwoWLKibN2/ybetfHDp0SFeuXLGui/Ttt9+qQoUKunTpkvbv36/x48dr69atqlmzpm7fvi0nJye+pHlKV69eVdasWXX06FGNGzdOgYGB1ispffHFFzKZTCpXrpw++ugjGydNP4KCgnT16lW1bt1a0p9lZWhoqPr27avt27crIiJCtWvX5rmaAqtXr9aaNWuULVs2+fj46KuvvlKzZs1UuHBh5c2bV0ePHtWgQYM4VkqBPXv2KCkpSbt375adnZ0qVaoks9ms+fPny8nJSVFRURoxYoQKFy5s66iPxSkhBvdgCnm1atUUHx8vFxcX3b59W9evX1fRokVVrFgxvf7665o7d66GDx+ufv36WS9Hx7TSJ/vrVNPFixfL3d1dNWrUUOfOnRUbG6vt27dry5YtKlCggLp06WLjxGnr4fG4dOmS1q5dq+TkZDk6OurVV1/V+++/r4sXL+rdd9/Vhg0b9MUXX3C+YAo8PK4HDhxQgQIFNGXKFP3vf/9TmzZtNGnSJNWrV0/fffedEhISlDVrVkqgxzCZTAoODta0adOUPXt21axZU9WqVVNycrLat2+vTz75RGvXrtW4ceP03XffKTo62taRDSkqKkru7u4ymUxaunSpduzYoUaNGuny5cvq27evhg0bpkmTJqlt27ZauHChdUFn/LuHX+8mk0kuLi4qVKiQZs2aZT3Q/uCDD9StWzf9+OOP6tmzJ2XFP8iePbvy5MljvaS4o6OjJk2apDx58mjcuHEym836+eeflT17dr366qu2jpuuWCwW3b59W2PGjFHJkiVVo0YNvfXWW5o/f77atm2rbNmyKSkpSWXKlFF4eLit4xraw6/3NWvWaNmyZUpISNDGjRs1depUubi46OrVq/L399eVK1c0fvx4yorHeHjR+y1btmjNmjUaMWKE3Nzc1L59ew0aNEirV6/W2rVrFRsbq8GDB6tgwYI2Tm18+/fv1+TJk7Vy5Uq9/PLLmjhxokJCQlSnTh3NmjVLv//+u7Jly2b45yWnhBico6Oj3nrrLTk4OGj06NEKDw9Xp06dNGXKFIWEhMjR0VEFCxZUgwYNdOvWLe3atUsS58CmxIMxOn36tC5evKgFCxbo66+/1vr16zVt2jR99NFHqlKlimJiYlS3bl0bp017D8Zj9erVWrdunbp3767s2bNrx44d2r9/vySpRo0aatq0qcxmM2VFCj0Y1++//179+/dXjx49NGfOHL366quaNm2aunfvrp49e2rx4sXKkycPZcVfXLp0SQcPHpT052t12rRpmjFjhnLkyKGlS5fqwIEDatWqlQYPHmydvRIXF6ezZ8+qePHiNk5vPMePH1fjxo21b98+3b59W6dOndKIESP07rvvqnXr1qpevbqmT5+uevXqacSIEcqZM6etI6cbD3942b59u2bNmqWwsDC9/fbbKlWqlCZPnqw7d+7o5s2bKlasmDp27GhdPA6PKlSokNzc3NSuXTvNmTNHH3zwgeLj45U/f35duXJFmzZt0tGjRzkd8RmYTCblzJlT9erV0/nz53XgwAEVLVpURYsWVZ8+fdStWzf17t1bRYoUUWhoqGJjY/92ygMefb2Hh4fr5s2bWrJkidasWSN3d3f1799fFSpUUJMmTZQ3b14NHjyY074e47ffftOgQYN09uxZSVJsbKwaNmyofPnyKXv27FqxYoVCQ0O1f/9+vfPOO2rVqhVlxWM8/Fo9e/asjh49qoiICJ0/f14uLi7q2rWr7O3t9d133+nEiRMqWLCg4csKicLC0B5cA9fFxUWRkZGKjY3VkiVL5OXlpebNm6t79+6aNGmSBg8erEaNGsnb21t37961cer05eLFi+rbt6+SkpLk4eGhIkWKaPz48dq4caNGjx6txo0ba/LkyXrhhRdsHTXNXL9+XX/88YfOnz+vGzduaN26dfL19ZWXl5c+/fRTubi4aPPmzerZs6emTp3KN4LPYNeuXTpx4oS2bdumzp076/Tp05ozZ45q1KihRYsWyWKx6K233mIxw7+wWCz6+uuv1atXL/388886deqU3nzzTZ08eVLh4eF66623rKcq3b59W++++65+//13jR8/XgMHDuTDzD9wcXGRg4ODtm/frjNnzljLWkny8vJSpUqVdO/ePcXExOidd94x9BRRo3nw4WXp0qVasWKFwsLC1KNHD129elX16tWTq6urWrVqpcDAQH366aeUk0+wceNGbdmyRd98842+++47bdiwQbNmzdJvv/2miRMnauXKlRozZoz8/PxsHTVdOXXqlAICAiRJjRo1Up06dXTs2DFdvHhRTZs21Zw5c9SyZUsdOXJEkydPVu/eveXs7MyXYH/xcFmxaNEitWnTRosXL9bixYslSdOnT1dSUpJ69eqlSpUqqWvXrhn6OPK/iouLU44cOTRv3jxdvHhRnp6emjx5ssLCwiRJ9vb2eumllxQfH2/jpMb34HkZFBSkXbt2qXr16qpRo4ZmzZqlX3/9VR4eHurYsaPy5MmTro6RODo2MDs7Ox06dEgLFixQlixZ9MUXXygxMVFBQUEqU6aMpkyZoqxZs+qLL75QdHS0fvnlF5UrV87WsdONXbt2ydPTU507d9avv/6q//3vf4qLi1OxYsUUGBioQ4cO6fbt2xn6Q+TevXs1cOBADRkyRF27dtXIkSNVpEgR/fDDDzp+/Ljc3NzUpUsXValSRfny5dOgQYM4yE6BhxvuP/74Q+vWrdPp06dlZ2en6tWrq0GDBjp9+rSmTJmiUqVKacyYMSpatKgNExuTyWRSo0aNlCVLFh08eFB58uRRtmzZ9OOPP+rrr79WmzZtVKZMGXl4eMjPz09+fn6qX7++Jk6cyHg+hp+fn0qVKqXDhw/r559/VuvWrRUXF6eZM2dKkm7cuKG7d+/q/v37Nk6afly6dMk6df706dPauXOnZs2apXLlyikqKkozZ85UlixZ9PHHH2vGjBmaOnUqRdBfXLx4UVeuXNHt27cVHByso0ePqnTp0ipbtqzGjBljvXz7uHHjNH78eI0f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Dg4O8vHxUa1ateTr66tdu3Zpz5496tOnDx8Gn0JkZKTGjBmjzp07Kzg4WD/99JM8PDzk4OCgpk2bat++fWrevHmmO45MqZMnTypbtmzKmzev5s+fr+DgYEVGRqpKlSpq3769/vjjD/Xu3VulSpWyrruAJ4uOjtbnn38uHx8flShRQvHx8fr111/18ccf69NPP1XRokWVP39+9evXL91/IcEMCxv6448/NGLECJ05c0b29vYym826c+eO9ecuLi7q0aOHnJycFBQU9MjPeIN5stjYWOufCxUqpObNm8vX11czZ85UXFycZs+erd27d6tTp04aNWqU6tSpkynfZGrXrq0BAwbom2++UVBQkH7++WctXrxYX3zxBWVFCplMJsXHx6tIkSJas2aNjhw5oqNHj6pMmTJasmSJLly4oKtXr6pGjRpq3LgxZUUKVKxYUW3bttW6deuULVs2zZgxQ61bt5ajo6POnz9v63jpUqVKldShQweNGzdO165dU8eOHbV79251797d1tHSjQdXsrhy5YrCwsK0fft2zZs3Tw4ODrpz546mT5+ue/fu6dNPP7Websd79ZPVqlVLAwYM0NChQ7Vq1SqNGzdOjo6OSkhIsF5BgLLi3124cEGjRo3Su+++q6ZNm6p48eIaOHCg4uPjVbp0aR07dkxTp07VihUr9M0336h27drKkiULz88n+Ov3udmyZVPt2rW1Z88e7dq1S5MnT1blypV1/PhxDRo0SO+9916mPI5Mqcw0GyAtnTp1Srdu3ZIkubq6qk6dOsqVK5defvllnT59Wh06dFDp0qXVsmVL1atXT23atEn3ZYXEDAubSkpK0pdffqmsWbPq/fffV58+ffTqq68qOjpapUuXVvbs2eXl5SVvb2+ZzWYVKlTI1pHThTNnzmjHjh2qX7/+IysKDxkyRIcOHdJLL72kjz76SH5+fjp9+rRy5cqVKU4DeZKdO3eqe/fuypUrl2bMmJEp1vH4r0JCQnT16lU1bdr0kRXVHyyO++ByccuXL5ckffPNN9bF45Ayu3fv1rx58/TBBx+obt26to6TIezdu1djx45Vt27dVLt2bVvHSTf27dunyZMnK3fu3IqNjVXZsmWVL18+/f777zp69Kh69uypUaNG6fz583r99dfVs2dP1v95CsHBwRo8eLD69+/Pa/0pxcbG6s0331S5cuWs6yNJ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KqlChQpasWKFDh48qHfffVdbtmzRiBEjVLBgQRunBgAAAACkFr6O/o9MJpP27NmjZcuWKVu2bCpUqJCaN2+unDlzasuWLYqLi9Mvv/yiLl26KH/+/LaOmy48XFaEhobqxo0bWrVqlUJCQnT48GElJCSoV69e2rZtm5KTkykrAAAAACADYg2L/+jEiROaMWOGAgMDZTabdfLkSTk7O6tChQry8PDQpEmT1KhRI8qKFHq4rFixYoVGjBihgwcPysfHR40bN1aZMmV04cIFLV++XPXq1dM777xDWQEAAAAAGRCFxX908eJFVatWTb/++quuXbumr776SmFhYcqdO7f69u2rxYsXq3r16uLMm5R5UFbs2rVL+/btU6tWrXTu3Dl9++23MpvNeuedd1SqVCldu3ZN8fHxNk4LAAAAAEgrnBLyFK5evaq9e/fq9u3bypkzp5o1a6b8+fNr9erV2rJli6ZOnSofHx+tWrVKjo6O6tChg/WKFSywmXJnzpzRxIkT1aZNG9WsWVO5c+dWt27dlJycrM8//1zvv/++7t69Kzc3N1tHBQAAAACkEQqLFLp06ZK++uorVaxYURaLRRs2bND58+dVoUIFFShQQPb29jpx4oRu3rypXbt2qW/fvpIoKlLir1dM8fLy0muvvabp06frhRdeUMmSJTVt2jR98MEHcnBwUJcuXSgrAAAAACCD4yohKXDhwgWNGzdOb7zxhho1aiRJioyM1Pjx4+Xu7q633npLe/fu1f79+2UymdSyZUtVr17dxqnTh4fLiq1bt+ry5csqXry4cubMqT179mjPnj3q37+/ihcvrtDQUJnNZtYDAQAAAIBMgMLiX8TGxurNN99UuXLlNGbMGElSfHy8HB0ddePGDX3wwQf68ssvrUVGRESEsmfPbsvI6dLy5cu1e/duVa5cWcuXL1fnzp318ssva9WqVdqyZYsCAwNVrFgxW8cEAAAAADwnLLr5L5ydndWrVy8dO3ZMP/zwgyTJ0dFR8fHx8vb2VrNmzRQaGmq9PWXF0wsLC9O+ffs0depUubm5qXDhwmrUqJFMJpOaNWumhg0bytXV1dYxAQAAAADPEWtYpED9+vVlb2+vgIAASdLbb78ts9ksSXJycrJltHTp+vXrMpvNunXrlooVKyZfX195e3ura9eusre318SJE3Xjxg3Nnj1bffr0UceOHVkLBAAAAAAyGQqLFKpdu7YkKSAgQMnJyXrnnXd0/PhxrV+/Xv369bNxuvRj7969WrBggbJkyaIzZ86oWrVqatSokTw8PHTmzBl16dJFJpNJx48f1+XLl3Xv3j25u7vbOjYAAAAA4DljDYuntGPHDgUGBqpu3bq6cOGCWrdurSpVqtg6VroQEhKib775Rr1791aRIkV09+5djRkzRn5+fnr55Ze1b98+Xbx4UQ4ODrpx44ZGjBihIkWK2Do2AAAAAMAGKCyewbZt29S3b1+NHz9eNWrUsHWcdGH//v3q27evli5dqjx58uj+/fvKkiWLrl+/rt69e+u1115Thw4dFBoaqt9++00vvvii/Pz8bB0bAAAAAGAjLLr5DOrWravt27erRo0aou9Jmfv37ys6Olrnzp2T9OfCpYmJifLx8dGgQYO0Y8cORUZGqmjRoqpXrx5lBQAAAABkchQWzyhHjhy2jpCu1KhRQ2PHjtXQoUO1Zs0amUwm2dnZKSEhQW5ubsqdO7fc3NxsHRMAAAAAYBAsuvkfcfWKlKtVq5YsFouGDx8ui8Wid955R3Z2djp27JiSk5OVkJCgLFmy2DomAAAAAMAAKCzwXD242srw4cOVPXt2ubq6avHixRo0aJBcXV1tnA4AAAAAYBQUFnjuateuLZPJpM8++0y5cuXSjBkzVLBgQVvHAgAAAAAYCFcJgc3s3btXfn5+KlSokK2jAAAAAAAMhsICAAAAAAAYDlcJAQAAAAAAhkNhAQAAAAAADIfCAgAAAAAAGA6FBQAAAAAAMBwuawoAAGzGYrFo/vz5WrFihRISEmQymVSlShX16tVLw4cPV758+dSlSxdbxwQAADbADAsAAGAzY8eO1caNGzVv3jzt2LFDP/74oxISEtSxY0dxITMAADI3LmsKAABsIjIyUtWqVdOaNWtUuHBh6/779+9r79692rx5swoUKKAuXbroyJEjCggI0L1792RnZ6cBAwbo9ddfV2JiooYMGaKff/5ZycnJKlasmEaNGiUnJ6d/3O/q6mrDfzEAAHgazLAAAAA2cezYMfn6+j5SVkhSlixZVKtWLdnZ/d9hyqBBg9SuXTtt3rxZHTt21ODBgyVJP/30k8LCwrR582Zt3bpVRYoU0ZEjRx67HwAApB+sYQEAAGzi7t27ypkzZ4pu+8MPP8hkMkmSKlSooLCwMElSjhw5dOHCBW3btk1VqlRRjx49JEnHjx//x/0AACD9YIYFAACwCV9fX12/fj1Ft123bp2aNWum+vXrq23bttb1LcqUKaMBAwZo0aJFqly5snr27Kk7d+48dj8AAEg/KCwAAIBNFC9eXHfu3NHJkycf2Z+QkKAJEyYoNjZWknT9+nUNGDBAX3/9tbZs2aJZs2Y9cvsGDRpo0aJFCgoKUmxsrObMmfPE/QAAIH2gsAAAADbh6uqqjh07yt/fX5cuXZIkxcbGatCgQTp9+rScnZ0lSbdv31bWrFlVsGBBJSYmasWKFZKk6OhorV69WlOmTJEkeXh4qFChQpL02P0AACD9YA0LAABgMx07dpSTk5M6d+6spKQkmc1m1apVS0OGDLEurFm8eHFVq1ZNtWrVkp+fn/z9/XX48GF98MEHWrhwob766ivVq1dPZrNZ+fPn16hRoyTpsfsBAED6wGVNAQAAAACA4XBKCAAAAAAAMBwKCwAAAAAAYDgUFgAAAAAAwHAoLAAAAAAAgOFQWAAAAAAAAMOhsAAAAAAAAIZDYQEAAAAAAAyHwgIAAAAAABgOhQUAAAAAADCc/wcrIrYlL4+UvwAAAABJRU5ErkJggg==
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>From this plot, we can see a close race between all the classes. Paladins seem to be falling behind, along with death knights, but is there any difference between specs?</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[4]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Spec&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Score&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">Dungeon92Ranks</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">(</span><span class="n">rotation</span><span class="o">=</span><span class="mi">70</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">&#39;seaborn-white&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;IO Score by Class (Top 10 players)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Spec&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Score&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">(</span><span class="mi">3000</span><span class="p">,</span> <span class="mi">4000</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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8cqVKxo8eLCOHDliXnfo0CFdvnxZVatWla+vr7Zu3ar4+Hilp6dr8ODB2rVrl55++mlt2rTJfFG7ePHi+47vIN3plrBs2TJlZGQoKytLM2fO1I4dO+772B07dig+Pl4ZGRnatGmTedDKMmXKyNPTU19++aXatm173207duyozMxMTZgwwTz2w+nTp/Xuu+/KxsYm22OvX78uLy8v5c2bV5cuXdL27duVnJwsSRo4cKDCw8MlSRUqVDB39/iz9XdzdnZWXFycuUXBn2nUqJFCQkLM3UcWL16sRo0aydb2zsRkO3fuNLc82Lx589+aySNfvnxq1KiRuUVHYGCgYmNjVa9evfs+fs2aNZKkM2fO6MKFC9kGQjXtqypVqsjKykq//fabbt68ad5X93tfihcvLnd3d61fv17SnVYkw4YNu29Xkl9//VXffPONpDutRMqUKZPt7zdu3Lhv1yQAAHID04UCAPAISpQooR9++EFTpkzR119/LWtra7m5uWnatGmqVavWPY+vWbOmxo0bpzFjxigxMVGZmZkqUqSIpk6dquLFi6t48eLq16+fnnvuOdnb26tJkyZq3769rKysNGDAAPXs2VOZmZmqVKmSxowZc9+aevbsqUuXLumZZ55RVlaWqlatqt69e9/3sc2bN9eQIUMUGRmpqlWrmscpkO7cnf/qq6/UokWL+25rY2Mjf39/ff755/Lz85ODg4MKFCig999//56uH927d9eQIUPk6+urqlWr6v3339fgwYM1b9489erVS8OHDzeP9/Diiy+qVKlSf7r+j/s/X758OnXqlCpWrHj/N0l3up2MGzfOPChk8eLFNW7cOPPfGzRooDfeeEMXL16Uj49Ptv1gsmjRIs2fP19JSUlKSkqSn5+ffHx89Nlnn2ns2LF67733tHz5cuXLl09ff/31Pa1lTJydnfXss88qISFBH3744T0tJt566y299tprcnV1Vffu3dWtWze9//77WrZsmTw9Pe95X6ysrDRlyhSNGTNG06ZNk7W1tfr27XvfriQtWrTQBx98oNatW8vGxkalSpXSpEmTJN0JRGJiYpguFABgGKush20LCQAA/hPWrl2rDRs26KuvvjK6lAf66KOP5ObmpjfeeOORth85cqQ8PT01aNCgf7mye3l7eysgIMA8C8ujyKn3ZcmSJQoICNDMmTP/1ecFAOBh0ZUD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SktLU1ZWlvl3yNIcPXpU27Zt0+LFi/Xzzz9r48aNOn36tG7evGl0afeVnp6u5cuXa8qUKRo6dKgyMjJkZ2cn6X8X2UYzfV8yMzMtpqY/Y2p1MmvWLH333XeSLOdc5H4sqTYrKyuLfX9Nx6EtW7bI39/f/JuT08dvunI8pM8//1zp6el6//33zetCQ0MVEBCgrKwsvf322wZWd4fpZHvz5s0KDAzUc889p2rVqhldlllmZqasra3166+/6vTp0/L19VXdunUVHx9v0eOFrF69WoGBgXJwcFD//v1VrFgxo0tSYGCg9u7dq4iICFlbW8vT01Ply5dX2bJl5eHh8Vh1OzL54YcfdPHiRXXp0kVVqlQxf14sRVpamnr37q3ChQvr2rVrKlCggHx8fDRw4EDZ29vnai0xMTG6fPmywsPDdeLECUVHRytv3ryqVq2a6tSpowoVKuRqPX9keu/mzJmjkydP6tSpUxo8eLBatGih27dvy9HR0dD6JCkhIUHjx49XUlKS0tPTNX36dN28eVOFChUyurQHMjU//vHHH2VjY6MmTZro66+/1hdffKFRo0apbdu2aty4sdFlZjNt2jQ1a9ZMNWvWNLqUe5h+N1NTU7VlyxaFhobKx8dHvr6+FnUcvXDhgpYtWyYXFxd1797dIr5D92PanxERERozZoxiY2OVnJysp59+Wp07d1b58uUNrW/btm0aP368qlWrpr59+6p69eoW2xrl2LFj+u6779S9e3c1aNDA6HIe6Pr16woJCVFYWJguX76sfPnyqVy5cipevLjq1atnced4ycnJGj58uA4ePKi6deuqbt26euaZZ1SkSBFt2bJFLVq0MKSutLQ0rV69WpGRkerUqZNKlixpSB2P4vTp0/ruu+/k6OioV199VSVLlrSI7jKmGg4dOqQ5c+YoMzNTnTp1Ur169QzpQmyqZ8WKFYqLi1OHDh1UqFAhxcbGysnJyaJ+dyQpODhYK1asUNeuXXPlN5xg4m/o1auXunTpovT0dC1YsEB58+aVl5eXevfurbJlyxpdXjbBwcH68ssv5efnp549e8rBwcEi+irGxcXplVde0SeffKJKlSrJxsZGn376qVq3bm1R072a9tXZs2c1efJkdejQQd98843Wrl2rX3/9VQ0aNFCJEiWMLlMJCQk6ceKEduzYocjISOXLl0+lSpVS7969c/1i+e8w7d/z588rPDxc+fPnl7OzsyZOnKisrCx99NFHKlOmjNFlSvrfRfbmzZu1a9cujRkzRpK0e/duffPNN3r22WfVrVs3Q2s8dOiQQkNDderUKRUoUEDvvfeeofVId/bbiy++qIULF+rll1/WhAkTdO7cOZ06dUovvfSSnJycDKvL2tpa8+fPV2ZmpsqUKaPff/9dX375pb744gu1bNky23TWlmrEiBHq1KmTNm/erNq1a6tdu3aaMWOG7O3tNWDAAIs43kvSvn371KdPH9WoUUN9+vRR/fr1VaBAAaPLMjN9HubNm6cNGzaoWbNmOnr0qGJjY1WmTBk988wzhl8Ummq8fv26vv/+e+3Zs0e9e/fWM888Y3EBhelzN2vWLMXFxWnkyJHatWuX1qxZox07dqhatWqaNWuW0WVq1apVunbtmpo2bWpx528mGRkZ2rZtm2bOnCkfHx8NGjRIbm5uFhXa312LqVVHYmKigoODFRgYqMTERI0ZM8Yix5Das2ePrl69Knt7e23btk2XL19WTEyMypQpY77zn1tMF6v+/v4KCAiQtbW1goODVaJECb3wwgvq2bOn8uTJk6s1PYrY2FitXbtWycnJevnlly3i+GQ6Jg0ePFhVq1ZVUlKSdu3aJUmqWrWqXnnlFUOOAX369FHfvn1VtWpVffbZZ7KyslLbtm3VrFmzXK/lQdLS0rRx40Z9//33atiwoQYOHKiCBQvm2HHI9l9/xifMDz/8oOTkZL3xxhvq06ePZs2apbJly+qtt95SnTp1LCLZMh3QTpw4oaSkJB0+fFjVqlXTiy++qLlz58rBwUE9e/Y09CTVdGDYvn27ypUrp6pVqyo9PV2S1KhRI61YscIig4nNmzerbdu2qly5smrXri0rKyvFxcXpt99+05AhQwypzfR+R0ZG6tChQypcuLDefPNNWVlZadmyZUpMTLToUEK6c2fqxo0b+uCDD1SlShWFhobK29tbzZo104EDB/T666/ryy+/VNWqVY0u1XzwvXr1qmxtbXXt2jU5OzurUaNGun79uvbt26du3brl+sni4sWL9dtvv6lBgwZ64YUX1Lt3b61Zs0ZeXl65VsODHDhwQOXLl1dcXJw5MCtQoIDmzZunPn36GFaX6T06ceKE+vbtqy1btujpp5+WdOe7dfDgQYsOJkzHpi5dumjFihU6duyYBg4cqDNnzigkJEQffvih0SWaZWZmqm7dutq6dau2bt2qGTNmaPr06apatar69etnEReEps9DQkKC3n//fVWvXl1Xr17VuXPntGXLFp06dcqwYMJ0rN+4caP27dunihUrqlevXipdurR+/vln3bp1Sz179jSktj9jOs/Ily+ffHx8JEmNGzdW48aNdePGDcXExOR6Tab9aOpSVrRoUV2/fl2nTp3Snj17VK1aNb355pu5Xtf93B0o2tjYqGXLlnr66ae1ceNGBQQEqEuXLhYTSkj/a+49f/58XbhwQSdOnFDDhg3Vvn17VahQQaGhoRYZSmRkZMjT01Nly5aVs7OzmjRpojNnzujChQuqUqVKrtdjalVw8uRJjR492nxjZsWKFfrqq690+fJlffzxx7le18MwdY3x9vY2dys+cuSI+vfvr7ffflu1a9c2NCi3srJSSkqKHBwc9Prrr0uS3n33XYWEhMjf31/Xrl3Ltd8i034IDQ1V4cKF1axZM02ePFlFihRRnTp19OOPP6pWrVqGf2fuPp+1t7dX+/bt1bp1a61du1abNm1S586dc+w4RDDxF1xdXbVt2zY1b95c+fPnV6FChTRw4ECLOfmX7jShc3Nz05w5c5Senq5SpUpp9uzZqlWrlvz8/LR06VKlpKTo1VdfNaxG0wHJx8dHISEhCgoKMgcR586ds6g7aNL/TlZtbW0VHR2tyZMn68UXX5Qk3bx509ALfxsbG2VkZOjtt99Wo0aNtGbNGhUtWlSNGzdWQkKC2rVrZ1htD8N0YD58+LBat25tvkhNTExU/vz51adPH23btk2rV69WlSpVDL/ra2trq5s3byo4OFiXL1/W3LlzValSJdna2iokJESdO3eWlDvNgE0/Fnv37tX27dvVp08fvfPOO5o7d65Kly6tPHny6JtvvsnxOh5G8eLF5eDgoAEDBqh+/fqS7rQycXFxsYjgzNfXV7NmzdLJkyc1Y8YMSXf6Snfo0MHgyv6c6QIrNTVVdevW1blz53T48GG9++67KlCggMqXL69y5cpJsoxm6RkZGeb+502bNtXKlSt17Ngxff/997l6MvhnTMeiq1evKjo6WpcuXVL16tXl7u4ud3d3+fj4mPueG8F0sRIQEKADBw7o+PHjCg0NVcWKFVWyZEmLHPBUutOke8mSJXJzc1NaWprKlSunIkWKyNnZWc7Ozrlej2k/BgcHa+HChRowYIBKlSql8PBwxcTEWNRYCKbv7ezZs3X06FFVq1ZNR48e1Y0bNxQREaEtW7Zo7NixKlq0qMGV3mFjY6OsrCytW7dO77//vo4cOaKoqCgNGTJEV69e1bhx44wuMRvTMfS3337TvHnzdPnyZdWqVUutWrVS48aNVatWrVyv6e4ZyvLmzau9e/cqX758cnNz03PPPafnnnvOIscXMdV96dIlBQcHa9WqVapTp44iIyNVuHBhlSlTRps2bVK1atUM+8031Xjy5EnFx8drypQpatu2rSpWrKg6derk+g1R0/c7IyNDZ8+e1cCBA1WkSBFNmDBBZ86cUaFChQwPJaT/XQN98MEHunHjhipWrKgDBw4oJSVFN27c0N69e/XRRx8pX758//pr05XjIV28eFH79+/XTz/9pNjYWDVo0EAdO3bUU089ZWhd+/bt04ABA9SuXTu98MILKlGihNzc3CTdGWXYzs5O6enpeuONNzR69GgVL17c0Hol6ZdfftH8+fPl5uamUqVK6cyZM/rwww8N73t6P6mpqfr8888VGBioV155RefOndOBAwc0depUQ04MTBem69ev18GDB9WlSxeNHz9ePXv21PTp01WwYEF9//33cnBwyPXa/q7Jkyfr6aefNl+0Snf2t4ODg3bv3q3Vq1dr4sSJBlZ45+SwWbNmKlWqlJycnBQeHq5169YpPDxcly5dUqVKldS6dWuVLl1apUqVyvF6TO//uHHj1KhRI2VmZurKlSvq2rWr3n//fdWvX9/wbiV3O3TokObNmycnJyddvnxZNjY2GjJkiGEtEkz7Lzw8XHnz5tWqVasUEhIiDw8PnTx5UhUrVtTYsWMNqe3v6NChgypXrqwXX3xR1atXV0REhAoWLGgOeI1u6m16/aVLl+ro0aNKS0tTamqqvvzySx06dEjVq1c3rLb72b9/v8aMGaPk5GRzt5h69eoZ3iLy7ruMJ0+e1JkzZ1S8eHGL2393M733YWFh2rt3r3bs2KF8+fKZj5UVK1Y0rLbbt29r6dKlWrt2rZ577jl16dJFcXFxsrGxsYiLgYyMDN28eVM2NjYKDAzU+fPnZWdnp4oVKyoiIkKenp7auXOnXF1d1atXL8O7a93dsnTTpk0aNmyYRo0apdmzZ2vWrFmqUqWKGjduLFtby7sHOmjQIL377rvy8vLSokWLtH79eh06dEgjRoxQjx49DKlpz549mjt3riSpTp06KlWqlEqWLCkvL68cuQD8p0zv/8yZM1W/fn3Vrl3b/LeMjAylp6drzJgx8vLy0oABAwys9M5NkcDAQF27dk358uVT4cKFVbx4cTVt2tSQsFS6EzifPXtWXbp0UWRkpKZNmyY/Pz8999xzhtRjcnfgtHbtWuXPn1/58+dX+fLldenSJbm7u2vFihUqX768+cbcv4lg4i9s375diYmJsrGxkZubmypUqGAehOrSpUvmg4gR7h4H4bffftP27duVmZmpOnXqqEOHDvLx8ZG9vb3i4+M1cuRIffvtt4bUaTpRSU5O1p49e+Ti4qISJUooPDxcKSkpqlOnjkUNOGeqNyIiQvHx8UpNTdWhQ4d05swZeXl5qVy5cob3AZs6darKly+vixcvys7OTq+++qqWLVumOnXqWFRrnj8TFRWlli1bysHBQX369NHLL7+crdXMjRs3lJGRIVdXVwOrvHMHvVKlSnrttdd0+fJl9erVSx06dJCTk5NCQ0O1ceNGXbx4UU8//bS6d++ea3V999138vT01OrVq9WhQwe1adNG3333nVq0aGHoXWjT3agzZ87o8OHDqly5shwdHRUREaH8+fOrRIkShp0E3G3cuHEaOnSo8ufPr8DAQCUnJ6tUqVJyd3e3iAuU+zEdly5fvqwlS5Zo3759SkhI0O3bt9WuXTu1aNHCIro+3e21117Thx9+qIULF6patWpq166dxo8fry5dusjb29vo8u5x48YNrVixQmvWrNHly5f1xRdfqFGjRobUYvouBQQEqHTp0kpKStLOnTt17Ngxubi46IUXXjCkyfnDuHr1qnbu3Klq1aqZ77TNnTtXXbp0MXebyi2m782lS5d07do1VaxYUXFxcZo3b57y5cunvn37Gh5AmVy/fl379+/Xjh075OjoeN9uWdHR0erXr59+/PFHFS5c2IAq73X48GGdOHFCiYmJiomJ0Xvvvad169YpIiLC8AvS+4mLi9PkyZM1YMCAbOdLERERcnBwMN/cM0poaKi2bt2qy5cv6/bt2+rbt69FDhwsSbdu3dLYsWO1b98+FS9eXDVq1JCfn58qVaok6c7NnSJFiuTIBezfkZ6ebm7Bd/bsWZ0/f16XLl3SiBEj5OHhkSs13N0NOzw8XImJiapVq5ZKlCih0NBQHT9+XJ07dza8RanpmDl9+nR5enrq2WefvecxYWFhGj9+vJYtW/avvz7BxJ+4ffu2vv76ax06dEi2trZyd3dXZmamvL29zU3PTS0SjPTHxPz8+fNatmyZtm/frtTUVH3xxReqUaOGYmJiDL/IGzx4sAoVKqR9+/YpIyND7dq10+uvv26RA/pkZWXp9ddfl4uLiz766CPZ29srMDBQtWvXNvygIUlnzpzRmTNnzD9cr776qvr166c+ffqoSZMmRpf3QHeP0hwcHKwZM2YoNDRUJUuW1DvvvGPYaNgPEh8fr6CgIK1atUpHjhxRxYoV1bFjR7Vr106HDx9W4cKFc3ww1LtPsG/duiXpzglhSEiI6tevr88//1wbNmwwbFDJuw0YMEAJCQmKjIxU+fLl1bJlS9WrV0/ly5c3/C7fkSNHNHjwYH3yySeGB4x/h+n9f+edd/T000/r6aeflp2dnZYtW6bFixcrLS1NLVu21IgRI4wuVdKdrlljx47VhAkTNGTIEPNgcr169dKoUaPMJ65GMe3PixcvauPGjQoJCVGePHnUtWtXNWjQQHv27FHlypUND82HDh2qqKgoNWzYUFZWVgoICND58+c1efJk+fr6Glrb3Uz7c9u2bVq6dKm5G6y9vb3ef/99tWzZ0tD6Zs6cqatXryosLEzlypVTyZIlNWfOHPXt21fDhw83tDaT1NRU7d69W5MmTZK1tbVatGihatWqqV69euabOtWqVdO8efP0xhtvGFprenq60tPTlZmZab5BYmdnpxEjRqhy5coKDw9X7969DX/f72fnzp2aO3eurK2t5evrqwoVKqhixYoqUKBArv8+3T2G1YYNG/T777+rdevWat++vVxcXLR69Wq1atXK4ro7m87jli1bpsuXL8vDw0P58+fX+vXrdebMGZUqVUqdOnVSs2bNZGNjY0gLPlONGzZsMJ+7+fn5qWnTpqpfv75OnjypypUr51o9ps9Wv379ZGdnJzc3NyUlJalQoULy9vZW+/btLSYklaQJEyYoKipKL7/8sqpUqZLt3DIiIkL79u3T888//6+/LsHEn1i1apV27dqlDz74QAULFlRMTIyCg4M1b948ValSRZ988onRJZoPaGfOnNGuXbsUGBgod3d3de/eXRUrVtTatWvVtGlTQ5uAmWoMDQ3VDz/8oOnTp0u60yz122+/Vdu2bdWmTRvD6vsjU72mEcQnT56szMxMpaSkmAdjfOGFFwypzXSQNfXT9/LyUmRkpPr06SM7OztVqlTJ3Ffe0oWGhio0NFQuLi7q2LGjbt68qblz58rNzU1du3ZVenq64c0/Tfv74sWLSkxMlJWVldzd3XXr1i1t2rRJR48e1WeffZbrdc2fP18pKSl6/fXXlZqaqjFjxsjOzk7Vq1c37LN5t8jISI0fP9488v7q1au1evVqhYSEaPny5fL09DSkrsuXL6tYsWKKjIzUrFmztHXrVrm6usrPz0/PP/+8xfTZfpCMjAz17dtXEyZMyDaN3IwZM1SvXj398ssvevnlly2m5YS/v79mzJghT09PzZkzR0ePHtXs2bP1888/G12a+Vg/efJkpaenq02bNjp58qQ2b96sZs2aqU+fPoZ1iTGdwGZkZCghIUHXrl3T+fPnVa1aNRUqVEhHjhxRjRo1DD9G3s20r95//301b95crVu3liRt2bJFW7Zs0dtvvy0XFxfDQsnz588rJSVF3t7eOnLkiFJSUpQ3b14VK1ZMLi4uhtT0ZwICAlSqVCmtW7dOQUFBcnJy0pkzZzRu3Dg1aNDA8HBXutNy49ChQ9q2bZuKFCmiYcOGSZJCQkK0dOlS1axZ07AuEX8lKSlJFy5c0L59+3Tp0iWlpqZKkrp3756rF6rS/743Y8aMkYuLiypXrqxVq1Zp586dGjBggEW2OLlb165dNXXqVBUvXlwpKSk6f/68li9frgIFCighIUGDBw82vGVPjx49NGHCBFlbW2vDhg3mmcL69euX67XcunVL48aN09ixY3Xt2jVzF72DBw/q9ddfNzywN0lKSpK/v7/OnDkjR0dHubq6qkyZMqpatap5HKucYjm/ahZmx44d6tSpkwoWLKj09HS5urqqffv2qlGjhqZMmWI+ybUECxculJ2dnXr16qXDhw9r/PjxeuGFF9SpUyfDB8wxndTt37/f3FwqPT1d3t7eevbZZ7Vy5UqLCiZM9d6+fds8Hoe1tbW5j+zp06cNq83UyuDXX3/VCy+8IG9vb5UpU0Y7duzQsWPHVKRIEcNqeximH+B9+/Zp3rx5KleunHbt2qUOHTroyJEj2e4AWcIJt2l/Dx06VA4ODipWrJhKlCihChUqqH79+uaTrtyep7tKlSqaNm2adu7cqQ8//FATJ05UUlKS4X1QTe/v2bNnVaBAAUVERKhkyZJq37692rdvbx7c1AiJiYnav3+/OZh466239PbbbyskJETr169XixYt9O2331p8ayPTKP29e/dWz5491blzZ2VkZGj9+vV64403NH36dIs5DqxYsUJ9+vSRh4eHNm/erA4dOqhBgwaGDsJ8N2tra2VlZSkoKEjLly+XlZWVatWqpTp16mjq1Klq2LChKlSoYEhtpgvPGTNmKCgoSBkZGfLx8dGNGzfUrVs3i5rBysTa2lqpqam6evVqtgEEW7RooYULF+rcuXO53mrz7ru6Z8+eVVxcnMqVK6eGDRuqQIECyszMtJhQ4u475ykpKVq9erX69u2r/v37KywsTLdv3zbPDmN0KCFJefPmNXcvKlKkiPLkyaPKlSuradOmysjIsIiWe3czfacSExMVEhKiyMhI1apVS61bt9b58+e1d+9eQ8Zgs7a2VmZmpk6ePKm3335bBQsWlK+vr27cuKEJEyZY1LXGH6Wlpalq1ar6+eef9eqrr8rZ2VmVK1fWtGnTNGbMGI0ePVqnT59W3bp1c7020/fp6NGjcnBwMM9y8tprr6l3794aOnSounfvnmstFEzHogsXLsjFxUW7d+9Wo0aN5O7urvr166t58+YW0Q3bVOfx48c1cOBASXfGMty/f78CAgLMx9CcZPzZvwW6evWqrly5ooYNG0q6c5F0+/Zt3b5929xcOzw83PCDhelEIDQ0VMuXL5ckNWzYUA0aNNCcOXNUp06dbHfVjNShQwd9/PHHmjVrlnnq0nXr1qlVq1ZGl3ZfTz31lObOnat9+/apRYsWatiwoTZt2qRevXoZWteNGzeUmZmpmTNn6vLly/Lx8ZG3t3eup/z/xC+//KIBAwbo6NGjcnJyMg+elZiYaDFNk69duyYXFxedP39elSpV0oQJE7R9+3YdOHBAW7du1fbt282tpnIjlLj7DlmdOnX0888/69dff9XmzZtVqFAhw49F0v9CvePHj+vy5cuaNm2aqlSpogoVKqhChQpyc3Mz7A702rVr5ejoqPPnz+v7779XhQoV5OXlpUqVKmn06NF655135O7unut1PYqXX35Znp6eWrp0qb7++mvVrVtXLVu21I4dO2Rra5tr/WUfJCoqSqtWrVLbtm3VokULc/hsCXd675aUlKRy5cpp9+7daty4saytreXt7a3k5GTDWvZId75LcXFx2r17t5Yu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u+/UrFkzde/eXQkJCQoJCVFKSorF3FVJSkrS4cOHdenSJZ0/f16vvPKKBg0apEGDBqlp06ZGl6eYmBht3bpV69atU2RkpEqVKqX+/fvrqaeeMrq0+0pKStKbb76pVq1aqVy5cqpQoYIKFiyoPXv2aOrUqUpLS1OfPn3UqVMni/jumOzZs0c///yzAgIC5OXlpRdffFEvvPCCOUg1WnJysubMmaOdO3eqevXqSk1Nlbe3t+zt7XX69GmNGjXKkLpMxx7T3bQxY8ZIknbv3q2JEyfq9OnT2rVrl0X0Rf4jUxP+vHnzKjAwUFeuXFFkZKScnJy0YMGCXK3l1q1bOnDggFJSUnT06FENGTJE58+f1/79+3X27Fldv35dr732mkWE+aZzy8zMTC1btkx58uTRqVOnlJCQIFtbWxUpUkTdunWzuIt9k4yMDC1fvlxz587V+fPn1ahRI33//fcWca78R88//7zatm2rrKwsbdq0SUlJSSpfvrzeeustwz4Ln332mQ4ePKhChQopKSlJjRs3lpubmwIDAzV58mRDanqQX3/9VUWLFlXFihWVN29e/fLLLzp9+rT279+vokWLqn79+howYIBFhKdffPGF8uTJo9DQUIWHh8vHx0cpKSkqX7683nvvvVytJSMjQ+3atZO7u7sGDx6smjVrWlTX64CAAG3btk1jxoxRVlaWrl27pnfeeUfz58+XlPvdTAgm7nLjxg19//33WrhwoYoVK6apU6eqYsWKRpeVzZkzZ/T999/r1KlTioiIUMuWLTVo0CCL6hZhOiglJCQoJiZGRYoUuae/odGtTu5mquXumuLi4rR3714tW7ZMjo6Omj59uiG19enTRyNHjlTFihWVmJiot99+WxERESpXrpxsbW3l7e2tQYMGGVLbwzDtU9M4Lc8++6xq1aqliIgIpaamqnz58uauSZb0mTANlHTr1i35+Pho4MCBWrJkia5du6bBgwcbciG4d+9e+fv7q1SpUho6dKhFXOiZvutxcXGKj483J/9vvfWW0tPTVaJECYscy+HMmTNaunSpypcvn6ujc/8d586dU79+/VS6dGk1bNhQtra2Kly4sLy9vZUnTx65u7vL1tbW8BNA6c6Jl6mOjIwM2dreaYy5fv16ff7552ratKlFzMZhcvToUVWuXFnR0dHauXOnjh49qnPnzqlJkyaGd9mbMWOG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ifr376+srCxNmjQpVy9cMjMzJUn79u2To6OjmjRpov79+6t///6qW7euunXrJm9v71yr50GaNm2q6OhoDRw4UMuWLVN4eLjWrVv32LTqsUSbN2/Wpk2bFBISojlz5mj9+vXq0qWLYmNj9d577+ncuXNGl5hNWlqaGjVqpEWLFik6OlpFixY1z4BiCRcspmPMgQMH9O233yokJERRUVGSJF9fX1WuXFm+vr6G1Wdtba0bN25o/PjxKly4sL799lu98cYbeu+99/T5558rIiLCsNoexM7OTn369NHBgwdVsGBBpaSkyNraWitXrjSk+6NJnTp1tGHDBs2YMUOurq4aNmyY6tevb24JaQlMgd67776rY8eOac6cOeratau5CXVuTWf4dzVo0EB79uzRunXrdPjwYa1du1YbNmxQ69atjS7tvhYtWqQDBw5o586dcnd3l6+vrwYNGqQhQ4aoYMGChtRkZWWldu3aafDgwdq8ebM55EtMTFS9evUMqelBTOcjK1askIeHh7Zv364JEybo2LFjGjp0qNzc3Mznyka33itatKiaNGmiPn36aO7cuTp37pwWLlwoDw+PXBtE1srKSoUKFdKgQYN08uRJvfHGGwoPD9fSpUvVrl075cmTR7dv386VWh6Fm5ubunfvruXLl2vs2LGS7lyT5BbGmND/Ej5Td4ixY8fq/fffV/PmzVW5cmWNGjVK8+fPt4i+0qYfhLtnBrhx44b279+vVq1aGVjZnbsUb731ls6cOaNSpUrphRdekJ+fn37++WdlZmZq+/btWr58ucX0NQ4NDZWdnZ3KlSsnBwcH3bhxQ3v37tXChQtVoUIF87422uM2m8DdTGHfiRMnVKlSJZUuXVoODg76/fffVbt2bZUrV84i+nWb7l6tWrVK8fHx6tmzp3lA1OTkZCUmJsrDwyPX7waMHz9eiYmJ6tmzp0qVKmXYidQf3T039+XLl9WkSRP98ssvOnnypIKDg9WuXTv16dPH0G5lj6uDBw+aW5q0b99eTZs2VWBgoGxtbVWsWDEFBwfr3XffVZUqVQy/O2X63gQGBpqbIC9btkw///yzPD09ZWVllW2MHKPt27dPixYtUkxMjNzc3FSrVi0dPXpU8fHxhjWbNx3/fv75Z6WkpKhRo0aaPXu2+vbtq6+++koVK1bUyJEjDant75g9e7Y2bNggd3d3FStW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
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>With this further delineation, we can see greater discrepencies between specialization performance over the last patch. Affliction warlocks have fallen off a cliff in terms of high end performance, while destruction warlock is excelling to be a top contendor. Without digging into specific spec analysis, one might assume warlocks to be a middle of the road class. The same can be said of Beast Mastery and survival hunters, who are facing a similar delima. One spec is soaring while the other tanks in IO score.</p>
<p>Before moving into the history of each class, we have yet to address another major component within the data set. One of the key selling features of the Shadowlands expansion for World of Warcraft was the Covenant system. Each player selects a faction (covenant) to join, and along with cosmetic rewards, they gain two additional abilties. One is covenant specific, and the other is class+covenant specific. The consequence of this, many players imagined, would be that high end players would be forced to select the "best" covenant in terms of player power instead of the covenant that felt was the most interesting. The data from the API contains covenant information for the top performers along with their scores. Let's take another look:</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Covenant&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Score&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">Dungeon92Ranks</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">&#39;seaborn-white&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;IO Score by Covenant&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Spec&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Score&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">(</span><span class="mi">3300</span><span class="p">,</span> <span class="mi">3700</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABCYAAAHtCAYAAADFvH/vAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAABArklEQVR4nO39e5zXdZ3//9/nwMhBAREGBhVTLAqPgXXRb4IKqKDV7npAEazEn66lVuJGpBkKIocC1JLMTwXKQoheXMktUVICipRKRMVsp8hVSg7KyQA5OO/fH36cTxNqbNubl4fr9Z9hnvN6v96P99A0b26+DhWlUqkUAAAAgAJUFj0AAAAA8N4lTAAAAACFESYAAACAwggTAAAAQGGECQAAAKAwwgQAAABQGGECAN5h+vTpk1/96leNnz/xxBMZOnRoevXqlRNOOCHnn39+Hn300Td9/FNPPZVPf/rT6d+/f0499dScc845Tfa3p4wYMSJTpkz5X+1j9erVGT58eHr37p1TTjkl//zP/5x77rnnHzRheW3fvj333ntv0WMAQOGECQB4B3vmmWdy0UUX5dxzz83ChQuzYMGCfO5zn8sVV1yRxx9/fJftS6VSLrnkklxwwQWZO3duHnjggVx44YW59NJLs3Xr1j3/Av4XNm/enCFDhuSAAw7IQw89lAcffDATJ07MLbfcktmzZxc93t/09NNPCxMAEGECAN7RpkyZknPPPTennHJKKioqkiTHHXdcPve5z2XixIm7bL9+/fqsXbs2Rx11VOPaKaeckjlz5qRFixZJkttuuy19+/bNqaeemrFjx6ZUKiVJ7rjjjpx22mnp379/PvvZz2bdunVJXjvyYezYsfnEJz6R+++/P9u3b8/111+fU089NX369Mmtt976pvOvXr06Q4YMyUknnZRLL700W7Zsyfjx4zNq1KjGbTZu3Jijjjqq8fled++992a//fbL5z//+TRr1ixJ0rVr19xyyy3p2bNnktfCzbnnnpv+/fvnn/7pn7Jo0aI0NDTkYx/7WJYvX964r2nTpuWKK65IksyePTv9+/dPnz59MmzYsLzyyiuNr/Pmm2/OBRdckJNOOikXXHBBY8xZunRpzjjjjPTv3z+nnXZaFi9enCRZuXJljj/++Nxxxx35xCc+kV69euXHP/5xXnzxxVx22WV5/PHHc9555731XzIAvMsJEwDwDvbLX/4yJ5100i7rJ510Un71q19l27ZtTdb33XffHHHEEfnUpz6Vu+66KytXrkySdOrUKUnyq1/9KnfffXfmzJmT++67L7/+9a8zd+7cPP744/ne976X6dOnZ+7cuencuXOT8PGLX/wid999dwYMGJDp06fnd7/7Xe67777853/+Zx544IHMnz//DedftGhRbr755vzkJz/Jxo0bc9ddd+XjH/945s6dm507dyZJ5s+fn2OOOSbt2rVr8tglS5bkhBNO2GWfH/zgB9O1a9c0NDRk2LBhGTJkSObOnZvrr78+V155ZbZs2ZJ+/frloYceanzMT37ykwwYMCBPPPFEbrrpptx+++15+OGHs/fee+emm25q3G7u3LmZPHly5s2bl3Xr1mXevHlJkq997Wu58MILM3fu3Fx88cUZOXJk42PWr1+fysrK3Hfffbnqqqty4403pn379hk2bFiOPvrozJw58w2/NwDwXiFMAMA72Msvv7zLP9iTpH379mloaMjLL7/cZL2ioiJTp07NySefnDvuuCN9+/bN6aefngcffDBJsnDhwpxwwgnZe++9U1NTk+nTp+eUU07JT3/605x66qnZb7/9kiRnn312fv7znzfu97jjjstee+2VJLn//vtz1llnpaamJi1btsw//dM/Ne7/r/Xu3Tvt2rVLVVVVTj755Dz++OM57LDDss8+++QXv/hFkteiwWmnnbbLY//85z+nffv2b/q9WblyZV588cWcfvrpSZIjjjginTt3zpNPPpn+/fvn4YcfTpKsW7cuzzzzTE444YTMnTs3ffv2TceOHZMkgwYNajL7CSeckLZt26a6ujof+MAH8sILLyR57eiNAQMGJEl69uyZ559/vvExO3fuzBlnnJEkOeyww/KnP/3pTWcGgPei6qIHAAD+fnV1dVmzZk26dOnSZP3FF19MdXV1Wrduvctj9tlnn3z+85/P5z//+bz44ou55557MmzYsMyZMyfr169PbW1t47avn96xbt26JuutW7fOSy+91Ph5mzZtGv/88ssvZ+LEifnWt76V5LWLPB555JFvOP9fRpV99tknmzZtSpJ8/OMfz3/+53/mIx/5SJYsWZIxY8bs8thOnTpl9erVb/q9WbduXfbZZ5/GU1xen3vdunXp379/Vq9enT/96U9ZvHhxTjjhhOy11155+eWXM2/evCxZsiTJa9fk2LFjR5MZX1dVVZVXX301SXLffffljjvuyObNm9PQ0NB4+svr27Vs2TJJUllZmYaGhjedGQDei4QJAHgHO+aYYzJv3rwcc8wxTdbnz5+fnj17pqampsn6qlWrsnLlysbt27dvn4svvjhz587N7373u+y7775Zv3594/av/7l9+/bZsGFD4/qGDRve9GiF2traDB069A1PMflrGzdubPzzpk2bGgPH6aefnoEDB6Z3797p0aNHk/Dxl6996tSpufTSS5vEh8ceeywrV67Mhz/84WzcuDGlUqnx6xs2bMh+++2Xqqqq9O3bN/Pnz8+iRYty1llnNc7+L//yL/nyl7/8N2d/3erVq/PVr341d911Vz70oQ/l2WefzamnnrrbjweA9zqncgDAO9ill16ae++9N/fdd1/j2pIlS3Lrrbfmi1/84i7bv/DCC7n00kvz1FNPNa498cQT+dOf/pTDDz88ffr0ycMPP5yNGzdm586dufTSS/Ozn/0sJ554YubNm9cYKmbNmvWG13dIXrud6V133ZVXX301pVIpU6ZMycKFC99w24ULF2bjxo159dVXM2/evMaLVh5yyCHp0qVLJk6c2HiKxF/75Cc/mYaGhowZMybbt29Pkvzud7/Ll770pVRVVeWAAw5Ip06d8uMf/zjJa8HixRdfbDx649RTT83DDz+cJ598Mr17926c/cEHH2y80OZPfvKT3HbbbW/8zf+/1q1bl5YtW+bggw/Ozp07c+eddyZ57VSTt1JdXZ0///nPTY6uAID3IkdMAMA72AEHHJDvf//7mTRpUm6++eZUVlamtrY2N954Y3r06LHL9h/+8IczevToXHvttXn55ZfT0NCQ/fbbL5MnT87++++f/fffPxdeeGH++Z//OTU1NenVq1c+/vGPp6KiIhdffHEGDx6choaGfOhDH8q11177hjMNHjw4f/zjH3P66aenVCrl8MMPz6c//ek33Pakk07K5ZdfnpUrV+bwww/PmWee2fi1008/PTfddFP69u37ho+tqqrKtGnT8vWvfz39+/fPXnvtldatW+crX/lK+vXrlySZNGlSRo4cmW9961tp0aJFbrrppsbTKo477rj827/9W3r37t14ZMlhhx2WSy65JOeff37j9+a66657y7+DD37wg+ndu3f69OmTurq6jBgxIo899ljOO++8TJky5U0f17Nnz3zjG99Ir169smDBglRVVb3l8wDAu1VFSaYHAN6GfvzjH+eBBx5oclcMAODdx6kcAMDbztatW/Pd7343559/ftGjAABlVvZTObZv357Ro0envr4+pVIp3bp1y8CBAzN+/PjGbTZt2pT27dvne9/7XubPn58pU6akWbNm6dChQ8aPH5/mzZtn2bJlGTt2bKqqqtKiRYtMmDDhDW+PBgC8s82fPz/XXXddzjzzzF0u6gkAvPuU/VSOhx56KIsXL84111yTJBkyZEg+85nPNJ77mST/9m//lk984hM59thjc9JJJ+Wuu+7K/vvvn+uvvz7t27fPJZdckgEDBmTMmDHp0aNHpk6dmhUrVmT06NHlHB0AAAAos7IfMdG3b9/Gi1Zt3rw5mzZtSseOHRu/vnTp0mzcuDEnnHBCHn300Rx88MHZf//9kyT9+/fPxIkT8/GPfzxbt25tvIjXgAEDMnDgwCbP88orr+Spp55Khw4dXDwKAAAA3kZeffXVrF27NocffniaN2/e5Gt77K4cI0aMyMKFCzN06NAcccQRjevf+ta38rnPfS5JsmbNmtTW1jZ+rUOHDlmzZs0u6+3bt8/atWub7P+pp57K4MGDy/wqAAAAgL/XjBkzdjlVc4+FiXHjxmXz5s255JJLcsABB6R///5ZsWJF1q1b13jP8r9WKpVSUVGxW+sdOnRI8tqL7NSp0z/+BQAAAAB/l1WrVmXw4MGN/3b/S2UPE8uXL0+LFi1yyCGHpFWrVunXr18effTR9O/fP/PmzWtyb/K6urqsWrWqyeCdOnV6w/W/PB0kSePpG506dcoBBxxQ5lcFAAAA/E+90aUXyn670GXLlmXSpEl5/RqbS5cuzaGHHpokeeyxx3LkkUc2bnvkkUfm+eefz3PPPZckmTNnTvr06ZO6urq0bds2S5YsabIOAAAAvLOV/YiJgQMHpr6+PoMGDUpDQ0O6du2as88+O0nywgsvNDmMo6amJuPGjcuVV16ZqqqqdOnSJUOGDEny2qkgo0aNSmVlZVq3bt3kdqMAAADAO1PZbxe6p6xcuTJ9+/bNQw895FQOAAAAeBt5q3+zl/1UDgAAAIA3I0wAAAAAhREmAAAAgMIIEwAAAEBhhAkAAACgMMIEAAAAUBhhAgAAACiMMAEAAAAURpgAAAAACiNMAAAAAIURJgAAAIDCCBMAAABAYYQJAAAAoDDCBAAAAFAYYQIAAAAojDABAAAAFEaYAAAAAAojTAAAAACFESYAAACAwggTAAAAQGGECQAAAKAwwgQAAABQGGECAAAAKIwwAQAAABRGmAAAAAAKI0wAAAAAhREmAAAAgMIIEwAAAEBhhAkAAACgMMIEAAAAUBhhAgAAACiMMAEAAAAURpgAAAAACiNMAAAAAIURJgAAAIDCCBMAAABAYYQJAAAAoDDCBAAAAFAYYQIAAAAojDABAAAAFEaYAAAAYI955JFHMmzYsDzyyCNFj8LbRHXRAwAAAPDeMW3atNTX12fLli059thjix6HtwFHTAAAALDHbNmypclHECYAAACAwggTAAAAQGGECQAAAKAwZb/45fbt2zN69OjU19enVCqlW7duGTlyZJ5++ulce+21qayszH777ZdJkyalZcuW6d27dw466KDGxw8aNCinnXZali1blrFjx6aqqiotWrTIhAkT0q5du3KPDwAAAJRR2cPEokWLUlNTk1mzZiVJhgwZkvnz52fy5MkZM2ZMjj766HzrW9/Kr3/96/Tq1Svbtm3L9OnTd9nPiBEjMmbMmPTo0SNTp07N5MmTM3r06HKPDwAAAJRR2cNE375907dv3yTJ5s2bs2nTptTW1qa6ujpHH310kuSyyy5LkjQ0NKSiomKXfaxcuTJbt25Njx49kiQDBgzIwIEDyz06AAAAUGZlDxOvGzFiRBYuXJihQ4dm5cqVqa2tzbXXXptnnnkmhxxySK666qqUSqXs3LkzV1xxRVavXp0uXbpk+PDhWbNmTWpraxv31b59+6xdu3ZPjQ4AAACUyR67+OW4ceMyb968LFiwIEnym9/8Jp/73Ofygx/8IJWVlbnttttSXV2dYcOG5dprr83MmTPTuXPnjBkzZpd9lUqlNzyyAgAAAHhnKXuYWL58eVasWJEkadWqVfr165c777wzhxxySGpra1NRUZE+ffrkmWeeSYsWLXLeeeelTZs2SV47ZWP58uWpq6vLqlWrGve5atWqdOzYsdyjAwAAAGVW9jCxbNmyTJo0KaVSKUmydOnS9OnTJ6tXr87q1auTJI899lje//735/e//30uuuii7NixI0myePHidO/ePXV1dWnbtm2WLFmSJJkzZ0769OlT7tEBAACAMiv7NSYGDhyY+vr6DBo0KA0NDenatWsGDRqUww47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6nZZ79ix4//kdQIA8DbX5siOefk3L2afD7UvehQA9qDdytGf+tSncuONN6ZFixZZvXp19tlnn9x0000577zz/uZjly1blkmTJqVUKiVJli5dmkMPPTRf/vKXG9cWL16c7t2758gjj8zzzz+f5557LkkyZ86c9OnTJ3V1dWnbtm2WLFnSZB0AgHePFgfsk9qTD06LA9764uoAvLvs1hETyWtHKVx++eWprKzMhg0b8vOf/zxHHnnk33zcwIEDU19fn0GDBqWhoSFdu3bN2Wefnfr6+px11lmpqalJ586dc91116Wmpibjxo3LlVdemaqqqnTp0iVDhgxJ8tqpIKNGjUplZWVat26d8ePH//2vGgAAAHhb2K0wMW7cuDz22GM58cQTs9deeyVJZs6cmSeeeCJf+cpX3voJqqubnLbxuje7o8fxxx+f448/fpf17t27N95yFAAAAHh32K1TOX76059mxowZjVGibdu2uf32292yEwAAAPhf2a0wsXPnzuzYsaPJ2tatW7N9+/ayDAUAAAC8N+zWqRwDBw7Mv/zLv+TEE0/MPvvskw0bNuThhx/OhRdeWO75AAAAgHexvxkmtm3blosvvjg9e/bMwoULs3Tp0qxatSoTJkzIMcccsydmBAAAAN6l3vJUjl//+tc54YQTsnr16vTs2TOHH354Hn300ey11175/Oc/33j7TgAAAIC/x1uGia9//esZPXp0OnbsmCS5+eab88UvfjH33HNPbr311tx44417YkYAAADgXeotw8T69etz8sknJ0n++Mc/pr6+PmeccUaS5Mgjj8xLL71U/gkBAACAd623DBNVVVWNf/7FL36Rbt26pV27dv/vwZW7dVMPAAAAgDf0lmWhtrY2CxcuzMaNG3PHHXc0Hj2RJE8//XT23nvvsg8IAAAAvHu9ZZj40pe+lKuvvjrHHntsmjdvns985jNJXrso5tChQ/Ov//qve2JGAAAA4F3qLW8Xethhh2XRokVZt25dk1M4DjjggNx66605+uijyz0fAAAA8C72lmHidX8ZJZKkY8eOjXfqeK/ZvuPV1DSr+tsbwnuUnxEAAOB/YrfCBP9PTbOqnDd8RtFj8H+9+OLLSZJVL77s7+VtYuaEwUWPAAAAvIO4rQYAAABQGGECAAAAKIwwAQAAABRGmAAAAAAKI0wAAAAAhREmAAAAgMIIEwAA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28/6um1+t8Mb2RM/66//W/31f7v/pbKHideNGDEiCxcuzNChQ3PEEUckSSZOnJj/+I//SP/+/XPKKafkvvvuS21tbeNjOnTokDVr1mTNmjVN1tu3b5+1a9c22f/rnw8ePHgPvBrgzfSdd3PRIwB7wuy+RU8A7AF9b/WzDu8Fo/vuuZ/1tWvX5qCDDmqytsfCxLhx47J58+ZccsklOeCAA9K/f/9ceeWVufzyy/OVr3wl3//+99OhQ4cmjymVSqmoqNhlX2+0fvjhh2fGjBnp0KFDqqqqyvpaAAAAgN336quvZu3atTn88MN3+VrZw8Ty5cvTokWLHHLIIWnVqlX69euXu+++OwceeGAOO+yw1NTUZMCAAZk9e3YuvvjiJqdirFq1Kp06dUpdXd0u6x07dmzyPM2bN88xxxxT7pcDAAAA/B3++kiJ15X94pfLli3LpEmTUiqVkiRLly7NSSedlJEjR2b79u1JksceeyyHHnpojjzyyDz//PN57rnnkiRz5sxJnz59UldXl7Zt22bJkiVN1gEAAIB3torS68WgTHbu3JkxY8bkN7/5TRoaGtK1a9dcd911ue2227JgwYJUV1enXbt2ueGGG9KmTZv87Gc/y0033ZSqqqp06dIl119/fWpqavL0009n1KhRqaysTOvWrTN+/Pi0adOmnKMDAAAA5VaCPez5558vfeADHyjNmTOnyfpJJ51UWrBgQWnKlClv+fgvf/nLpdmzZ++yvmXLltIDDzxQKpVKpZ07d5bOPffc0sCBA0vbt2//xw0P/K88//zzpV69ejV+vn79+tInPvGJ0kMPPbRbj7/++utLTz75ZLnGA3bTW/0uL5eTTjqp9Oyzz/7dj+/Vq1fp+eef/wdOBO89gwYNKs2bN6/J2tatW0vHHHNM6YUXXvgf7evee+8tlUq7vjfgvansp3LAG3nf+96XW265JX/+85+brPfu3Tuf/exn/659Pv3003nwwQeTJGvWrMl///d/584770yzZs3+1/MC/3hbt27NJZdckqFDh+726XlXX331G14wCdjz3ux3OfDuddZZZ+Xee+9tsjZv3rwcffTR6dSp027v59VXX82UKVP+wdPxTrbH7soBf6m2tjbHH398pkyZkuHDhzeu33PPPVm8eHG+8Y1vZMGCBZk4cWLatGmTU045Jf/n//yfLFy4MEny29/+NpdcckmeffbZnHHGGfnUpz6Vq6++Ops2bcqECRPy9NNPZ9OmTTn//PPzve99L6NHj86KFSuyY8eOHHnkkfnqV7+aJPnxj3+cf//3f0+zZs3SunXrjBo1Kvvuu28h3xN4L9m5c2e+8IUv5PTTT88///M/Z/LkyWnWrFkuu+yyJMltt92WjRs3pnnz5vnjH/+YP/7xj/nyl7+c8ePH57Of/WyOPfbYjBw5cpef65UrV+azn/1sjj/++DzxxBPZvHlzvvOd7+xywWTgf+/NfpcnyaRJk/LYY4+loqIihx9+eIYPH56KiopMmTIlDz30UCorK/NP//RPGTJkSM4///x88IMfzG9+85vcfvvtWbRoUW655ZY0b948LVq0yOjRo5v8DL/66qu54YYbsnz58iTJsccemy9+8Yt59NFH8+1vfzs1NTU55ZRTcuKJJ+aLX/xiqqqq8sEPfrDxemfA32/AgAGZMGFC1q9f3/ie+d57782ZZ56Zr371q/nv//7vNDQ0pG/fvhk6dGjje/uGhob84Q9/yP77759vfvObueqqq/LHP/4xQ4cOzahRo5IkkydPzi9/+cts3bo1t956a2bOnLlb7w38B4t3B0dMUJgLLrggCxYsyIoVK3b5WqlUysiRIzNhwoRMnz49a9eubfL1l156KbfeemumTZuWb3/722nevHkuvvji/H//3/+X4cOH5/rrr0+7du0yffr0bN68Od26dcuMGTMye/bs/OxnP8t//dd/5YUXXmjcx+23355jjjkm3/nOd/bUy4f3rFKplKuuuiqvvPJKzj///CTJ2WefnR/+8IeN/3CYO3duzjzzzCTJ888/nzvuuKPJG4+NGze+4c91kvz+97/PGWeckRkzZuRDH/pQ7r///j38CuG9441+l99///1ZvXp1/v3f/z3Tp0/Pc889l/nz5+dXv/pVfvrTn2b27NmZMWNG5s+fn02bNiVJWrZsmX//93/P9u3b89WvfjXf/OY3M3369PTu3Ts33nhjk+e8//77s3LlyvzgBz/IjBkz8vOf/7zxAulPPvlkJkyYkLPOOit33HFHjjrqqNx+++355Cc/mTVr1uyx7wu8W7Vo0SInn3xyfvSjHyV57Sjl3/72t1m5cmVqa2szffr03HHHHfnRj36UZ555JslrNz+44YYbcs899+SZZ57Jb37zm1x++eVp165dvv/97ydJXnzxxZx++umZOXNmunfvnh/96Ef/4/cGvLM5YoLC1NTUZPjw4RkzZky+973vNfna+vXrs3Xr1nzwgx9MkpxyyilNDhv76Ec/miTp1KlTtmzZkldfffVNn6d169Z54YUXcs4556SmpiZr167N+vXr87vf/S5r167NhRdemCTZvn17DjjggH/wqwT+2osvvpj3v//9qa+vzw9/+MN88pOfzAEHHJAuXbrkl7/8ZTp16tR4m+kkOeqoo1JRUdFkH2/2c92yZcvsu+++ef/7358k6dy5czZs2LCnXyK8Z7zR7/JHH300jz/+eGN4fPnll7Ny5crs2LEjPXv2TFVVVaqqqpr87u/Ro0eS5Nlnn81+++3XeEj4Rz/60cyaNavJcy5btizHHXdcKioqUlVVlWOOOSZPPvlkDj/88Bx88MFp27ZtkuS//uu/MnDgwCTJYYcdln322aes3wt4rzjrrLMyatSoDBkyJD/84Q/z8Y9/PL/85S+zatWq/PKXv0zy2vvq1++0eOSRR6Z58+ZJkrq6umzcuDGtW7duss999903H/jAB5K89v5+06ZN/+P3BryzCRMU6oQTTsgPfvCDzJs3r8n6Xx9uWVVV1eTz6uqm/9N9q8Mzf/SjH+XJJ5/MjBkzUl1dnTPOOCPJa2+mjjzySEdJwB7WoUOHXHTRRenfv38GDx6crl275rDDDsu5556be++9NwcddFDOOuusxu3f6Doxb/Zznez6/xcO34by+uvf5TU1NRk4cGBj+H/d97///Tf9eXyz60GVSqW/+Y+Pv9zmL/dTKpVSWfn/Dg5+q/+IAey+o446Ktu3b8/vf//7zJkzJ5MmTcqNN96YSy+9NP3792+y7T333LNbv5ffbJv/yXsD3tmcykHhrrrqqkycODHbt29vXNt3331TWVnZeGjo6xe1fCuVlZXZtm3bLusvvfRS9t9//1RXV+epp57Kc889l+3bt+eII47IE0880XiayP3335+f/OQn/6BXBfwtBx54YK6//vpcfvnlWbduXU488cQ8+eSTefjhh3d5Y/PX3uznGijGX/4u79mzZ+bNm5edO3cmSb71rW/l2WefzYc//OH84he/yI4dO7Jz586cf/75u5xecfDBB+ell17Kn/70pyTJL37xixx11FFNtvnwhz+cxYsXp1QqZefOnVmyZMku2yRJ165ds3Tp0iSvHWWxZcuWcrx0eE8688wzM2XKlLRs2TLvf//707Nnz8ydOzdJ0tDQkLFjx77lEYtv9r79r/1P3hvwziZMULguXbrk1FNPbXIdicrKylx11VW59NJLc+GFF6ampmaXoyT+2hFHHJGlS5fmK1/5SpP1/v375+mnn86QIUPy4IMPZujQobn++uvTvHnzXH311fnXf/3XDB48OHfffXeOPvrocrxE4E307t07Z555Zr7whS8kSXr16pVu3bqlRYsWb/m4N/u5fv18dWDP+svf5aeccko+/OEP59xzz83AgQPz0ksv5cADD8yHP/zhnHLKKRk8eHDOO++89OvXL7W1tU3207x584wZMyZXXHFFzj///PziF7/IF7/4xSbb9O/fP126dMmgQYMa99OzZ89dZvr0pz+dRx99NJ/61Kfywx/+MAceeGA5vwXwnvLJT34yDzzwQOM1HwYPHpwWLVrknHPOycCBA7PPPvs0nlb1Rmpra9OxY8ecccYZ2bp165tuV11dvdvvDXhnqyg5xpW3qZ/85Cfp1q1bDjzwwDz44IO58847d7kWBfDusX379px33nkZN25cDj300KLHAQAK5r3Be4drTPC21dDQkMsvvzx77713Xn311Vx77bVFjwSUyYIFC/KNb3wj55xzjjceAID3Bu8xjpgAAAAACuMaEwAAAEBhhAkAAACgMMIEAAAAUBgXvwQA9oinnnoqX//617N69eqUSqW0bds2X/rSl3LMMccUPRoAUCAXvwQAyq5UKqVXr165/vrrc+KJJyZJHnzwwVxzzTX56U9/6v70APAeJkwAAGW3bt26HHfccXnkkUey7777Nq6vWrUqixcvzv3335+2bdvm8ccfT+vWrTNx4sS8733vy8svv5xRo0bliSeeyM6dO/O5z30uZ555ZpJk0aJFGTduXHbu3Jn3ve99GT9+fNq2bVvQKwQA/l6uMQEAlN2+++6bI444Ip/61Kdy1113ZeXKlUmSTp06JUkWL16cwYMHZ968eTn++OPz9a9/PUkyefLkVFZW5v77789dd92Vb37zm/mv//qvbNmyJVdeeWUmT56cBx54IF26dMlNN91U2OsDAP5+wgQAUHYVFRWZOnVqTj755Nxxxx3p27dvTj/99Dz44INJkq5du+boo49Okpx66qlZunRpkuT+++/Pueeem8rKyrRr1y4nn3xyHnzwwTz22GOpq6vLBz7wgSTJl770pXzlK18p5LUBAP87Ln4JAOwR++yzTz7/+c/n85//fF588cXcc889GTZsWK666qq0adOmcbvWrVtn06ZNSZKXX345w4cPT1VVVZJk27Zt6d+/f9avX5/WrVs3PqampmbPvhgA4B9GmAAAym7VqlVZuXJl4x042rdvn4svvjhz587NK6+8kg0bNjRuu3HjxsZQUVtbm1tuuaXxyIjX/exnP8v69esbP9+6dWs2btzYeGoIAPDO4VQOAKDsXnjhhVx66aV56qmnGteeeOKJ/OlPf8qWLVvyhz/8IU8//XSS5IEHHkjPnj2TJH369MmsWbOSJDt37swNN9yQ5cuXp2fPnlm7dm2eeOKJJMmUKVNyyy237OFXBQD8I7grBwCwRzz44IO57bbb8vLLL6ehoSH77bdfvvCFL+SFF17If/zHf6Suri6PPfZY2rRpkxtvvDEHHnhg/vznP+e6665rDBC9evXKV77ylVRVVWXJkiW55pprkiQHHXRQxo0bl3bt2hX5EgGAv4MwAQAU6p577skPf/jDTJs2rehRAIACOJUDAAAAKIwwAQAAABTGqRwAAABAYRwxAQAAABRGmAAAAAAKI0wAAAAAhREmAAAAgMIIEwAAAEBh/v9Bl1Qr3vKg9AAAAABJRU5ErkJggg==
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>We can see a close cut between covenants in the top performers, but honestly this does not tell us much of value. Players seem to prefer Venthyr, but we cannot attatch any specific reason just by looking at this plot.</p>
<p>To address this, we can identify the number of top 10 players for each class and covenant, and each spec and covenant pairing.</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[6]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">covenant92Data1</span> <span class="o">=</span> <span class="n">Dungeon92Ranks</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Class&#39;</span><span class="p">,</span> <span class="s1">&#39;Covenant&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">size</span><span class="p">()</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="s1">&#39;Count&#39;</span><span class="p">)</span>
<span class="n">covenant92Data2</span> <span class="o">=</span> <span class="n">Dungeon92Ranks</span><span class="o">.</span><span class="n">groupby</span><span class="p">([</span><span class="s1">&#39;Spec&#39;</span><span class="p">,</span> <span class="s1">&#39;Covenant&#39;</span><span class="p">])</span><span class="o">.</span><span class="n">size</span><span class="p">()</span><span class="o">.</span><span class="n">reset_index</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="s1">&#39;Count&#39;</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[7]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Class&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Count&#39;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">&#39;Covenant&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">covenant92Data1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">&#39;seaborn-white&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Covenant Representation by Class&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Class&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Count&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">(</span><span class="n">rotation</span><span class="o">=</span><span class="mi">70</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">bbox_to_anchor</span><span class="o">=</span><span class="p">(</span><span class="mf">1.05</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span> <span class="n">loc</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span> <span class="n">borderaxespad</span><span class="o">=</span><span class="mf">0.</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>

<span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Spec&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Count&#39;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">&#39;Covenant&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">covenant92Data2</span><span class="p">,</span> <span class="n">dodge</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">&#39;seaborn-white&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Covenant Representation by Spec&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Spec&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Count&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">(</span><span class="n">rotation</span><span class="o">=</span><span class="mi">70</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">bbox_to_anchor</span><span class="o">=</span><span class="p">(</span><span class="mf">1.05</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span> <span class="n">loc</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span> <span class="n">borderaxespad</span><span class="o">=</span><span class="mf">0.</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABKQAAAIqCAYAAAAaSZJCAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAABxiklEQVR4nO3dd1yVdeP/8TczENyKOHCm4B64c4UD3As1B5lmNszb0tIys7Qy9c601KYr9x5Z7j1z771CQUFUFBAQOFy/P/pyfnlXBgLXAX09H48ej9vrnHOd97nuwxnv8/l8LjvDMAwBAAAAAAAAJrG3dQAAAAAAAAA8XSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQDAU8swDM2cOVMBAQFq2rSpmjVrpo8//lgxMTG2jpYqa9as+dusISEh8vb2VkBAgAICAuTv768WLVpo3LhxslgsNkiafosXL07z9Xr37q1Tp05lyP1PnjxZH3zwQbr2ER0drdGjR6tJkyZq3ry5WrVqpRkzZsgwDEmSn5+fDh48mBFxAQAAsjwKKQDAU+uLL77QmjVrNHPmTG3evFk///yzEhMT1b9/f2tJkJV9/fXX/1ieOTg4aN26dVq3bp3Wr1+v5cuX69ChQ1q2bJnJKdMvIiJC06ZN+9frWSwWjR8/3vrvn376SRUrVszMaKmWnJysV155RQ8ePNDatWu1ceNGzZgxQ7/++qsmTZpk63gAAACmo5ACADyV7t69qzlz5mjs2LEqXLiwJClHjhwaOXKk+vXrJ8Mw9ODBA40cOVL+/v5q2bKlxo4dK4vFonHjxunTTz+17isyMlLVqlVTdHS0Ll68qF69esnf319t27bViRMnJEn79u1Tt27dNGHCBLVs2VJ+fn7av3+/JCkuLk5vvfWW/P395efnp3Hjxln3HRQUpJkzZ6p79+5q2LChBg8eLMMw9P777+vKlSsKCgpK1agad3d31alTR2fOnJH0x2idd999V/7+/mratKm1qAoJCZGvr6+mTZumNm3aqEWLFtq0aZMkafny5XrzzTfVu3dva/GzePFiBQQEyM/PT4MHD1Z8fLwkaf/+/erYsaNatWqlli1bau3atY+8X0ny9vbWypUr1aFDBzVo0ECzZs2SJL3wwgu6fv26AgIClJCQoCNHjqhTp04KCAhQq1attGfPHklSnz59FB0drYCAAF27du2hEUdr165VmzZtFBAQoBdffFFXr16V9MfIp9GjR2vAgAFq2rSpAgMDdfPmzb89hvfv39err74qPz8/BQUF6datW5o7d65effVV63WSk5NVv359nT179qHb7tixQ+Hh4fr444/l6uoqSfL09NTEiRPVtGnTv9zXkiVL1LJlS7Vo0UI9e/ZUaGioJCk8PFy9e/dWq1at1KxZM02cOPGR2wEAALIsAwCAp9C2bduM5s2bP/I633//vfHKK68YiYmJRlxcnNG5c2dj5cqVxtGjR43nn3/eer2lS5car776qmGxWIw2bdoYixcvNgzDMA4ePGg0aNDASExMNH777TejUqVKxsaNGw3DMIwff/zReOmllwzDMIzp06cb/fr1M5KTk427d+8atWvXNg4cOGAYhmH06tXL6NWrlxEXF2fcv3/fqFevnnHw4EHDMAyjXLlyxo0bN/6S+9q1a0b58uUf2hYWFmYEBAQYq1atMgzDMEaNGmUMHTrUsFgsxu3bt43GjRsb586dM65du2Z4e3sb06ZNMwzDMHbv3m3UqVPHSExMNJYtW2ZUq1bNuHLlimEYhnHs2DGjfv36RlhYmGEYhvHhhx8aY8eONQzDMDp16mTs27fPMAzDuHLlijF48OBH3m/K4/nvf/9r3XflypWNpKQk47fffjOaNWtmfSxt2rQxfvnlF8MwDGPFihXWy/73cT///PPGgQMHjNDQUMPX19f4/fffrce7d+/ehmEYxtdff23Uq1fPCAkJMZKTk43+/fsb33zzzV+O6ddff21Ur17duHr1qmEYhjFkyBDjs88+M27dumVUqVLFuHPnjmEYhnHgwAHD39//L7cfN26c8cEHH/xl+5+l5L1165ZRqVIl6/+37733njF8+HDDMAxj7NixxuTJkw3DMIzY2Fjj7bffNsLDw/9xOwAAQFbFCCkAwFMpOjpa+fPnf+R1tm3bpq5du8rR0VEuLi5q27atdu/erapVq8owDOsomI0bN6ply5a6fPmyrl69qs6dO0uSfH19lS9fPh05ckSS5ObmpmbNmkmSKlasqOvXr0uS+vbtq2+++UZ2dnbKnTu3ypYtq5CQEGuOgIAAubi4KEeOHCpZsqRu3Ljxr4/PYrFY15Bq0qSJOnXqpJ49e6pdu3aS/hgx9MILL8je3l758uVT8+bNtWHDBkl/rK0VGBgoSapfv76SkpIUHBwsSSpZsqRKliwpSVq3bp2aNm2qQoUKSZK6d+9u3Uf+/Pm1cuVKXbp0SSVLltSECRP+9X4lqX379tbj8+DBA92+ffsvj23lypVq2bKl9Rhfu3btkcdi9+7dqlOnjkqUKCFJ6tKli/bt26fExERJUs2aNVW0aFHZ2dmpfPny/3h8fX195eXlJemP/0+OHj2q/Pnzq2bNmlq/fr2kP54LrVq1+sttY2Ji/vX5liJ//vw6dOiQPD09rflSHmP+/Pm1a9cuHTx4UM7Ozvryyy/l4eHxj9sBAACyKkdbBwAAwBY8PT0VHh7+yOvcuXNHuXPntv47d+7c1oKkefPm2rx5s4oXL67Dhw/riy++0Pnz52WxWB4qJGJiYnT37l3lypVLOXPmtG63t7dXcnKyJOn333/X2LFjdfnyZdnb2yssLEydOnWyXtfd3d36vx0cHFK1MHnKGlKSdOnSJfXo0UOtW7e2Xh4dHa2hQ4fKwcFBkvTgwQMFBARIkrUYS5ErVy7du3fPegz+vI+NGzdapx4ahmEtecaMGaNvv/1Wffr0kYuLiwYPHqyAgIBH3q8k6zFKuTzlGP3Z6tWrNXv2bN2/f1/Jycn/ut5XZGSkcuXK9dB9GIahu3fvPnSfKff7T8c3X758D+0j5Zi0bt1ay5cv1wsvvKDNmzfr22+//cttPT09/7U4S2GxWDR58mRt3rxZFotF9+/fV6lSpSRJL730kpKTkzVq1CjdvHlTPXv21MCBA/9xu52dXaruEwAAwGwUUgCAp5KPj4+ioqJ08uRJVapUybo9MTFRU6ZM0WuvvaYCBQpYSwvpj3WnChQoIEny9/fXmDFjVLZsWdWqVUvu7u7y8PCQm5ubtQj6s3379v1jltGjR6tixYqaOnWqHBwc9MILL2TcA5VUpkwZPf/885o6dapGjBghSfLw8NDUqVNVrly5h64bEhIiwzAUGRmpvHnzSpLu3bv3UBGVwsPDQx07dtSwYcP+clmBAgX04Ycf6sMPP9SuXbs0cOBANWzY8B/vN7XCw8M1YsQILVmyROXLl9fvv/8uf3//R94mf/781lFqKY/H3t7e+vhSK6WAkqSoqCjlyZNHktSiRQuNHj1a27dvl6urq8qWLfuX29aqVUvz5s1TfHy8XFxcrNuvXr2qzZs3q0+fPtZta9as0ebNmzV37lzly5dPixcv1urVqyVJjo6O6t+/v/r3768rV67olVdeka+vr5577rl/3A4AAJAVMWUPAPBUcnd3V//+/fXee+9Zp6PFxcVp5MiROn36tFxdXdW4cWMtXbpUFotFsbGxWrVqlRo3bixJqlGjhm7fvq3ly5dbp48VLVpUnp6e1kLqzp07Gjx4sGJjYx+Z5fbt2ypfvrwcHBy0e/duBQcH6/79+//6GBwdHRUVFZWqx/vmm29q2bJl1sfq5+enhQsXSpKSkpI0ZswYnTp1ynr9X375RZK0a9cuubi4WEfo/Jmfn582bNigO3fuSJI2bdqkH374QYmJiQoKCrIuDl6xYkU5OjrKwcHhX+/3nx5nbGyskpKSdOfOHeXIkUOlSpVSUlKSFi1aJOmPkWhOTk5KTk7+y5kHn3vuOR08eNA6QmnhwoV67rnn5OiYtt/lDh06ZJ1muW7dOvn6+kr647nUsGFDjRo1yvpc+F+1atVS+fLlNXToUGu+sLAwvfXWW0pKSnrourdv31bRokWVN29eRUZGas2aNdbnw8iRI7V7925JUvHixVWgQAHZ2dn943YAAICsikIKAPDU6t+/v7p27arXX39d/v7+6ty5s/Lnz68pU6ZIkl588UV5enqqdevW6ty5s5o0aWItHOzs7NSsWTPt3btXzz//vHXbl19+qXnz5ikgIEC9evVSvXr1lCNHjkfmeP311zVmzBi1atVK+/fv15tvvqlJkybp0KFDj7xdQECAXnjhBa1Zs+ZfH2uxYsXUqVMnffHFF5Kkt956S9HR0fL391fr1q2VnJwsHx8fSX9MW0tMTFTr1q318ccf69NPP5W9/V8/MlSsWFGvvfaagoKC1LJlS82aNUtNmzaVk5OTAgMD9dJLL6lVq1YKCgrSiBEj5OLi8sj7/Sfe3t7KnTu3nnvuOeXKlUuNGjWSn5+funXrJj8/P1WrVk09evRQwYIF5evrq+eff16HDx+23t7T01OffPKJ3njjDbVs2VIHDhzQ6NGj//WY/S8/Pz998sknatq0qW7duqV+/fpZL2vdurVCQ0P/sZCSpK+++koeHh7q0KGDAgIC9Prrr6t79+565ZVXHrpemzZtdPfuXT3//PMaMmSI3n77bYWFhenTTz/VCy+8oIkTJ1rPMFi9enXVq1fvH7cDAABkVXbGvy28AAAAnhohISFq0aKFTp8+beso2crx48c1evRoLV261NZRAAAAsgVGSAEAAKRDUlKSpk6dqqCgIFtHAQAAyDYopAAAAB7T6dOn1bx5c3l4eKhdu3a2jgMAAJBtMGUPAAAAAAAApmKEFAAAAAAAAEyVtvMdmyg+Pl4nT55UwYIF5eDgYOs4AAAAAABAksViUUREhCpVqiQXFxdbx0E2lWULqZMnT6pnz562jgEAAAAAAP7GvHnzVLNmTVvHQDaVZQupggULSvrjCe7p6WnjNAAAAAAAQJLCwsLUs2dP6/d24HFk2UIqZZqep6enihUrZuM0AAAAAADgz1heB+nBouYAAAAAAAAwFYUUAAAAAADA/0lItGSr/WZXWXbKHgAAAAAAgNmcnRzUY+i8DN/v/PGpO3FbSEiIevTooR07dkiS7t69qxdffFFvvfWW/Pz8/vX2n332mdq3b69KlSqlK29mo5ACAAAAAADIguLi4vTaa6+pb9++qSqjJOmDDz7I5FQZg0IKAAAAAAAgi0lKStKgQYPUunVrdejQQRMnTpSTk5PefPNNSdIPP/yge/fuycXFRaGhoQoNDdWwYcM0btw4vf7666pbt64++ugjXb58WYmJiapSpYpGjBihkJAQvf7662rQoIGOHz+u+/fv6/vvv1ehQoVMfXysIQUAAAAAAJCFGIah4cOHKz4+XkFBQZKkLl266Oeff5ZhGJKkdevWqXPnzpKka9euafbs2Q9N07t37568vb01b948LV68WLt27dL58+clSZcuXVKnTp00b948lS9fXmvXrjX5EVJIAQAAAAAAZCm3bt1S2bJlFR0drZ9//lmSVKxYMRUvXlwHDhzQ1atX5erqqtKlS0uSqlatKjs7u4f2kStXLt24cUPdunVTUFCQIiIiFBkZKUnKmzevypYtK0kqUqSI7t69a96D+z9M2QMAAAAAAMhCChYsqFdeeUUBAQHq2bOnypQpo4oVK+qFF17QypUrVaJECQUGBlqv7+Tk9Jd9/Prrrzpx4oTmzZsnR0dHderUyXqZg4PDQ9dNGXVlJkZIAQAAAAAAZEFeXl769NNPNXDgQN25c0dNmjTRiRMntGXLFgUEBDzytrdv31bRokXl6OiokydP6urVq0pISDAp+b9jhBQAAAAAAMD/SUi0aP74npmyX2cnh3+/4v9o1KiROnfurEGDBmnmzJlq2LChYmJi5Orq+sjbBQQEaOXKlerVq5dq1Kihvn376tNPP9XEiRMf9yFkKDvDFuOyUiEkJERNmzbV5s2bVaxYMVvHAQAAAAAA4vu6LSUkJKhHjx4aO3asnn32WVvHSRem7AEAAAAAAGRx27dvV+fOndWhQ4dsX0ZJTNkDAAAAAADI8ho3bqzGjRvbOkaGYYQUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAACBdEpISs8Q+gIyQnEnPxdTuNyQkRN7e3vr5558f2u7n55cZsaz7Dg4OfuzbN2rUSCEhIWm6DWfZAwAAAACki7Ojk16aOShd+5jV56sMSgOkj72jkw6N75fh+/UdOi3V1y1ZsqSmTp0qPz8/ubu7Z3iWrIBCCgAAAAAAIAvx8PBQgwYN9M0332jo0KEPXfbll1/q8OHDsrOzU6VKlTR06FDZ2dnpm2++0ebNm2Vvb6/27durV69eCgoKko+Pj86cOaOffvpJO3fu1NSpU+Xi4iJXV1d98sknKlSokHXfFotFY8aM0alTpyRJdevW1VtvvaV9+/bp22+/lbOzs1q0aKEmTZrorbfekoODg3x8fGQYRpofI1P2AAAAAAAAspg+ffpo+/btunz5snXb2rVrFR4errlz52rOnDm6evWqtm7dqoMHD2rbtm1avHix5s2bp61btyoqKkqSlCNHDs2dO1cJCQkaMWKEJk+erDlz5qhRo0aaNGnSQ/e5du1ahYSEaMGCBZo3b552796t/fv3S5JOnDih8ePHKzAwULNnz1bVqlX1008/qV27drp582aaHx+FFAAAAAAAQBbj7OysoUOH6rPPPrNu27dvn44ePaqgoCAFBQUpNDRUISEhOnbsmHx9feXg4CBnZ2dNnz5duXLlkiTVqFFDkvT7778rf/788vT0lCTVrl1bJ06ceOg+jx07pnr16snOzk4ODg6qWbOm9TqlSpVSnjx5JEnnz5+Xr6+vJKlixYrKmTNnmh8fU/YAAAAAAACyoMaNG2vBggXauHGjpD9Kqq5du+rll19+6HozZsz4x2lzTk5Of7vdMAzZ2dk98v7/fJ0/78cwDNnb//8xThaL5d8fzP9ghBQAAAAAAEAWNXz4cE2YMEEJCQny9fXVxo0blZSUJEmaMmWKfv/9d1WvXl179+5VYmKikpKSFBQU9JdpdKVKldLt27d1/fp1SdLevXtVtWrVh65TvXp17dmzR4ZhKCkpSfv37//LdSSpTJkyOnLkiKQ/RlXFxsam+XExQgoAAAAAACCLKl68uPz9/fXdd9+pRYsWOnr0qF544QXZ29urYsWK8vLyUsmSJdWiRQv17NlTktS6dWt5eHg8tB8XFxd99tlnevvtt+Xs7KwcOXI8NB1QkgICAnT48GF1795dycnJatasmXx9fbVv376Hrte7d28NGjRIL774osqWLSsvL680Py4743GWQjdBSEiImjZtqs2bN6tYsWK2jgMAAAAAeISXZg5K1+1n9fkqg5Igsz3p39eTkxJl7/j309yy4n6zK6bsAQAAAAAA/J/MKo0oox5GIQUAAAAAAABTUUgBAAAAAADAVBRSAAAAAAAAMBWFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAAD8n4SkxGy13+zK0dYBAAAAAAAAsgpnRye9NHNQhu93Vp+vUnW9kJAQNW3aVP/973/Vrl0763Y/Pz99/PHHOnXqlF5//fV/vP17770nX19fdenS5aHtcXFx2rlzp1q0aCGLxaJevXopOTlZc+fOlZOT0+M9qHRghBQAAAAAAEAWUrJkSU2dOlUxMTEPbW/UqNEjy6hHOX36tDZs2CBJunnzpoKDg7Vo0SKblFEShRQAAAAAAECW4uHhoU6dOumbb755aPvy5cv1zjvvSJK2b9+udu3aKSgoSHPmzFGjRo2s1zt37pxee+01BQQE6IcfflB8fLw++OAD7dmzR+PHj9f777+vqKgoBQUFKSEhQR9++KF69uyprl276tNPP7XuZ82aNerRo4d69+6tgQMHKjIyMsMeI4UUAAAAAABAFtOnTx9t375dly9f/stlhmHoo48+0vjx4zVnzhxFREQ8dPnt27f13XffadasWfr222/l4uKi/v37q379+ho6dKg+/fRT5cuXT3PmzNH9+/fl7e2tefPmafHixdq1a5fOnz+vGzduWPfx008/qWbNmvr+++8z7PGxhhQAAAAAAEAW4+zsrKFDh+qzzz7T9OnTH7osMjJScXFx8vHxkSS1aNFCK1eutF5eu3ZtSZKnp6diY2NlsVj+8X5y5cqlGzduqFu3bnJ2dlZERIQiIyN18eJFRURE6OWXX5YkJSQkqFixYhn2+CikAAAAAAAAsqDGjRtrwYIF2rhx40PbDcN46N8ODg4P/dvR8eG653+v/2e//vqrTpw4oXnz5snR0VGdOnWS9EchVqVKlQwdFfVnTNkDAAAAAADIooYPH64JEyYoISHBui1v3ryyt7e3TudLWaz8Uezt7fXgwYO/bL99+7aKFi0qR0dHnTx5UlevXlVCQoIqV66s48ePW6cDrl27Vps2bcqgR8UIKQAAAAAAAKuEpETN6vNVpuzX2THtZ7QrXry4/P399d1331m32dvba/jw4RowYICKFCmimjVr/mVU1P+qXLmyvvjiC73//vsaMGCAdXtAQIBWrlypXr16qUaNGurbt68+/fRTLV68WB988IFeffVVubq6ysXFRePGjUtz/n9iZzxq3JYNhYSEqGnTptq8eXOGzlEEAAAAAGS8l2YOStftM6MAQObg+3rWsGnTJnl7e8vLy0sbNmzQokWL/rLWVFbGCCkAAAAAAIBsJjk5WQMHDpS7u7ssFos+/vhjW0dKEwopAAAAAACAbKZFixZq0aKFrWM8NhY1BwAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAA+D+WhESb7bdHjx7atGnTQ9vi4+NVq1YthYWFpen+Vq1aJUkKCQlRo0aN0nRbM3CWPQAAAAAAgP/j4OykNS/2yfD9tpo981+vExgYqJUrV6pZs2bWbRs3blS1atXk6emZ6vuyWCz65ptv1L59+8fKagYKKQAAAAAAgCygZcuWGj9+vCIjI5U3b15J0sqVK9W5c2eNGDFCwcHBSk5OVtOmTdW3b18tX75ce/bsUXJysq5cuaKiRYtq8uTJGj58uEJDQ9W3b1+NHj1akjRx4kQdOHBAcXFx+u677zR//nw5OTnpzTfflCT98MMPunfvnlxcXBQaGqrQ0FANGzZMlSpVypTHypQ9AAAAAACALMDV1VXNmzfXr7/+Kkm6efOmzp07p5CQEHl4eGjOnDmaPXu2fv31V509e1aSdOTIEY0ZM0bLly/X2bNndebMGQ0cOFD58uXTjBkzJEm3bt1S69atNX/+fFWoUEG//vqrunTpop9//lmGYUiS1q1bp86dO0uSrl27ptmzZ2daGSUxQgoAAAAAACDLCAwM1OjRo9WrVy/9/PPPatOmjQ4cOKCwsDAdOHBAkpSQkKCrV69KkqpUqSIXFxdJUuHChXXv3j3lypXroX3mzZtX5cqVkyR5enoqKipKxYoVU/HixXXgwAF5enrK1dVVpUuXliRVrVpVdnZ2mfo4KaQAAAAAAACyiKpVqyohIUGXLl3SqlWr9OWXX2rSpEkaMGCAAgICHrru8uXL5eDg8NC2lBFPf/ZP13nhhRe0cuVKlShRQoGBgdbLnZycMurh/COm7AEAAAAAAGQhnTt31jfffKMcOXKobNmy8vX11bp16yRJycnJ+vzzz3X37t1/vL29vb0ePHjwr/fTpEkTnThxQlu2bPlL2ZXZKKQAAAAAAACykHbt2mn9+vXWNZ169uwpV1dXdevWTV27dlXOnDmVJ0+ef7y9h4eHChUqpE6dOikuLu4fr+fo6KiGDRvK29tbrq6uGf0wHsnO+LuxXFlASEiImjZtqs2bN6tYsWK2jgMAAAAAeISXZg5K1+1n9fkqg5Igsz3p39ctCYlycM74KWuZtd/0SEhIUI8ePTR27Fg9++yzpt43I6QAAAAAAAD+T2aVRlmtjNq+fbs6d+6sDh06mF5GSSxqDgAAAAAA8NRp3LixGjdubLP7Z4QUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATOVoxp1MnDhRe/bsUXJysnx9fTV8+HAtWbJEixYtkqOjo3x8fDRy5EjZ29OPAQAAAAAAPOkyvQHatm2bDh06pEWLFmnJkiU6dOiQ9u/fr8mTJ2vGjBlauHChbt68qV9//TWzowAAAAAAACALyPRCqkGDBvr+++9lb28ve3t75cmTRydPnlTdunWVK1cuSZK/v7+2b9+e2VEAAAAAAACQBWR6IeXo6Cg3NzdJ0rFjx3TlyhXFxsbKw8PDep2CBQvq5s2bmR0FAAAAAAAAWYBpizYdPHhQQ4YM0eTJk+Xo+PDSVYZhyM7OzqwoAAAAAAAAsCFTCqn9+/frww8/1Pfff6+KFSvK09NTYWFh1svDwsLk6elpRhQAAAAAAADYWKYXUnfv3tXIkSP1448/qkyZMpKk5557Tvv371dkZKSSk5O1evVq+fn5ZXYUAAAAAAAAZAGO/36V9Fm6dKmio6P1/vvvW7e1a9dOQ4YMUb9+/eTo6Khq1aqpRYsWmR0FAAAAAAAAWUCmF1L9+vVTv379/vay9u3bZ/bdAwAAAAAAIIsxbVFzAAAAAAAAQKKQAgAAAAAAgMkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAICnhCUhMUvsA8iqEhItWWIfwNPA0dYBAAAAAJjDwdlJa17sk659tJo9M4PSAFmPs5ODegydl659zB/fM4PSAE82RkgBAAAAAADAVBRSAAAAAAAAMBWFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAADAVBRSAAAAAAAAMBWFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAADAVBRSAAAAAAAAMBWFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAADAVI5m3ElERISGDBmixMRELViwQBaLRdWqVVO1atWs1xk4cKBq165tRhwAAAAAAADYkCmF1ODBg9WwYUNt3bpVkhQdHa0iRYpozpw5Ztw9AAAAAAAAshBTpux9++23qlq1qvXfMTExcnNzM+OuAQAAAAAAkMWYMkLK3d39oX/HxMTo7t27GjBggG7fvq1KlSppyJAhcnV1NSMOADyWhKREOTs62XwfAAAg/XhfBwDbMqWQ+l/58+fX66+/rrZt28rJyUkjRozQt99+q8GDB9siDgCkirOjk16aOShd+5jV56sMSgMAANKD93UAsC2bnGWvYMGC6tKli1xcXOTg4CB/f3+dOnXKFlEAAAAAAABgMpsUUnv37tWwYcNkGIYkac+ePapQoYItogAAAAAAAMBkmT5l7/r16xo2bJiioqIUEhKioKAgNWzYUK6urgoMDJSzs7OKFCmiUaNGZXYUAAAAAAAAZAGZXkgVKVJEc+bMyey7AQAAAAAAQDZhkyl7AAAAAAAAeHpRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBSDLS0i0ZIl9AAAAAAAyhqOtAwDAv3F2clCPofPStY/543tmUBoAAAAAQHoxQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgp4giUkJWaJfQAAAAAA8GeOtg4AIPM4OzrppZmD0rWPWX2+yqA0AAAAAAD8gRFSAAAAAAAAMBWFFAAAAAAAAEyVqkJqyJAhf7u9S5cuGRoGAAAAAAAAT75HriG1ZcsWbdmyRTt37tSHH3740GVRUVG6evVqpoYDAAAAAADAk+eRhVTVqlUVFxenTZs2qVChQg9dVrRoUfXr1y9TwwEAAAAAAODJ88hCKn/+/GrdurVKlSqlChUqmJUJAAAAAAAAT7BHFlIpYmNj9fLLL+v69etKTk5+6LL169dnSjAAAAAAAAA8mVJVSL333nvq3r27KlSoIAcHh8zOBAAAAAAAgCdYqgopZ2dnvfzyy5mdBQAAAAAAAE8B+9RcqVmzZtq6dWtmZwEAAAAAAMBTIFUjpPbv369Zs2bJ3d1dOXPmfOgy1pACAAAAAABAWqSqkBo8eHBm5wAAAAAAAMBTIlWFVIkSJTI7BwAAAAAAAJ4SqSqkGjduLDs7OxmGIUmys7OTvb293N3dtW/fvkwNCAAAAAAAgCdLqgqps2fPPvTve/fuadmyZXJzc8uUUAAAAAAAAHhypeose/8rd+7c6tu3rxYuXJjReQAAAAAAAPCES9UIqfDw8If+nZycrLNnz+r27duZEgoAkHkSEi1ydnKw+T4AAAAAPL0eaw0pe3t7eXh4cPY9AMiGnJ0c1GPovHTtY/74nhmUBgAAAMDT6LHWkAIAAAAAAAAeV6oKKcMw9Msvv2j37t26ffu2ChQooCZNmsjf3z+z8wEAAAAAAOAJk6pCavz48Tp48KDatm2rXLly6e7du/r+++914cIFvfnmm5mdEQAAAAAAAE+QVBVSO3bs0PLly/XMM89Yt3Xt2lVdunShkAIAAAAAAECa2KfmShaLRc7Ozg9tc3FxUXJycqaEAgAAAAAAwJMrVSOkateurddff11du3a1TtlbunSp6tatm9n5AAAAAAAA8IRJVSE1fPhwzZ49W9OnT9edO3fk7u6ugIAABQUFZXY+AAAAAAAAPGEeOWUvJiZGvXr10m+//ab+/ftr3rx5Wrt2rerXr6/9+/eblREAAAAAAABPkEcWUl9++aVKliyp+vXrP7R94MCBypcvn6ZMmZKp4QAAAAAAAPDkeWQhtWvXLo0YMeIvC5o7Ojpq5MiR2rJlS6aGAwAAAAAAwJPnkYWUYRhycXH528tcXV1lsVgyJRQAAAAAAACeXI8spBwdHRUeHv63l129elX29o+8OQAAAAAAAPAXj2yUunbtqv/85z/6/fffH9p++vRpDRgwQN27d8/MbAAAAAAAAHgCOT7qwj59+ujWrVtq3769PD09VaBAAYWHhysqKkr9+vVTr169zMoJAAAAAACAJ8QjCylJevfdd9W/f38dPXpUMTEx8vT0lLe3t9zd3c3IBwAAAAAAgCfMvxZSkpQ7d241btw4s7MAAAAAAADgKcCq5AAAAAAAADAVhRQAAAAAAABMRSEFAAAAAAAAU1FIAQAAAAAAwFQUUgAAAAAAADAVhRQAAAAAAABMRSEFAAAAAAAAU1FIAQAAAAAAwFQUUgAAAAAAADAVhRQAAAAAAABMRSEFAAAAAAAAU1FIAQAAAAAAwFQUUgAAAAAAADAVhRQAAAAAAABMRSEFAAAAAAAAUzmacScREREaMmSIEhMTtWDBAknSkiVLtGjRIjk6OsrHx0cjR46UvT39GAAAAAAAwJPOlAZo8ODBatCggfXfYWFhmjx5smbMmKGFCxfq5s2b+vXXX82IAgAAAAAAABszpZD69ttvVbVqVeu/9+zZo7p16ypXrlySJH9/f23fvt2MKAAAAAAAALAxUwopd3f3h/598+ZNeXh4WP9dsGBB3bx504woAABkOclJiTa9fVaSkGix6e2Bf5IRzy2enwAA/H+mrCH1bwzDkJ2dna1jAABgE/aOTjo0vt9j39536LQMTGNbzk4O6jF03mPffv74nhmYBvj/0vvclHh+AgDwZzZZRdzT01NhYWHWf4eFhcnT09MWUQAAAAAAAGAymxRSzz33nPbv36/IyEglJydr9erV8vPzs0UUAAAAAAAAmCzTp+xdv35dw4YNU1RUlEJCQhQUFKTGjRtryJAh6tevnxwdHVWtWjW1aNEis6MAAAAAAAAgC8j0QqpIkSKaM2fO317Wvn37zL57AAAAAAAAZDE2mbIHAAAAAACApxeFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAADAVBRSAAAAAAAAMBWFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAADAVBRSAAAAAAAAMBWFFAAAAAAAAExFIQUAAAAAAABTUUgBAAAAAADAVBRSAAAAAAAAMNVTX0glJyWmex8JSQkZsI/05wCA7CS9r3u8bgKZLyM+J2XEPgAAwJPH0dYBbM3e0UmHxvdL1z58h07TSzMHpWsfs/p8la7bA0B24+zolK7XTl43gcyXUZ+TAAAA/tdTP0IKAAAAAAAA5qKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKTxxLQmKW2AcAAAAAAPh7jrYOAGQ0B2cnrXmxT7r20Wr2zAxKAwAAAAAA/hcjpAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAAAAAAGAqCikAAAAAAACYikIKAAAAAAAApqKQAgAAAAAAgKkopAAAaZaclGjrCAAAAACyMUdbBwAAZD/2jk46NL5fuvbhO3RaBqUBAAAAkN0wQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqRxtdcfBwcHq3Lmzypcvb902atQolS5d2laRAAAAAAAAYAKbFVIxMTGqUqWKZsyYYasIAAAAAAAAsAGbTdmLiYmRm5ubre4eAAAAAAAANmKzEVLR0dH6/fff9dprr+nu3buqV6+eBg4cKHt7lrUCAAAAAAB4ktms/Xn22Wf1yiuvaMqUKfrpp590/PhxLVmyxFZxAPwDS0JiltgHAAAA/ioh0ZIl9gEAaWWzEVIlS5ZUyZIl/wjh6Cg/Pz+dOnXKVnEA/AMHZyetebFPuvbRavbMDEoDAACAP3N2clCPofPStY/543tmUBoASD2bjZBatWqVvvjiC0mSYRjau3evKlSoYKs4AAAAAAAAMInNRkg1a9ZMW7duVbdu3WQYhipVqqTAwEBbxQEAAAAAAIBJbFZIubm5adKkSba6ewAAAAAAANgIp7QDAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAAAAAYCoKKQAAAAAAAJiKQgoAAAAAAACmopACAAAAAACAqSikAAAAABMkJyXa9PZPEo4FAGR/jrYOAAAAADwN7B2ddGh8v8e+ve/QaRmYJntL77GUOJ4AYGuMkAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAIAtJSEq06e0BMzjaOgAAAAAAAPj/nB2d9NLMQY99+1l9vsrANEDmYIQUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwFYUUAAAAAAAATEUhBQAAAAAAAFNRSAEAAAAAAMBUFFIAAAAAAAAwVbYupBISLbaOAACwEUtCYpbYBwAAyBjpfV/mfR3IXhxtHSA9nJ0c1GPovHTtY/74nhmUBgBgJgdnJ615sU+69tFq9swMSgMAANIrve/tvK8D2Uu2HiEFAAAAAACA7IdCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopWCUkWtK9D0tiQrr3kZyUmO59ZAXpPZ4ZcSzx/z0pzysASK2MeF8HMgvPTzzJ0vu5k8+teFo42joAsg5nJwf1GDovXfuYP76nDo3vl659+A6dlq7bZxXpPZ4cy4xl7+jE8QTwVMmo93UgM2TE5yQgq0rv504+c+JpwQgpAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKgopAAAAAAAAmIpCCgAAAAAAAKaikAIAAAAAAICpKKQAAAAAAABgKkdb3vnUqVO1fft2GYahxo0b680337RlHAAAAAAAAJjAZoXUsWPHtG7dOi1btkyS1L17d9WvX181atSwVSQAAAAAAACYwGZT9nbs2KFmzZrJ2dlZzs7Oatq0qbZv326rOAAAAAAAADCJzUZI3bx5UxUqVLD+u2DBgjp8+LD13xaLRZIUFhb2yP08iL2brhwhISGKiI5P9z7i78amex9ZQVY5nul154HtM0jpO55Z6bmZFY5nVnlu8rf+h6xwPLPKczOjpOd4ZqXHkRHS+9qJ/y+r/K0/KWx9PDPqWGaV184n5XNSVpARz82MYOvPnVnhuZmSIyP+1tP7OSkzpXxPT/neDjwOO8MwDFvc8YcffqgKFSqoe/fukqTFixfr6NGjGjNmjCTp4MGD6tmzpy2iAQAAAACAfzFv3jzVrFnT1jGQTdlshJSnp+dDo5/CwsLk6elp/XelSpU0b948FSxYUA4ODraICAAAAAAA/ofFYlFERIQqVapk6yjIxmw2QurUqVMaOnSoli9fLknq1KmTxo4dq8qVK9siDgAAAAAAAExisxFSFStWVMeOHdWzZ0/Z2dmpU6dOT1wZZRiG7OzsbB0DAAAAAAAgS7HZCKmnRVJSkhwdHZWcnCx7e5ud1BAAAAAAACDLoCHJJMePH9exY8f0ww8/KCYmxlpGJScn2zhZ9pTSm967d09Hjx4VPeq/279/v+Lj03f2GTws5e/3+PHjslgs/D1nEP6ekdXxHE0/wzCUmJho6xhPHJ6byEpSzrZ2+/ZtGyfJ/lL+tu/cuSOJ75B4clFIZQKLxSJ7e3vNnj1bS5Ys0aZNm3TmzBklJibK3t5eoaGhto6Y7aS8KC9ZskSnT5+2ToU0DIMX6L/x+++/a8aMGRo9erR++uknnTt3ztaRngj29vYyDEM//fSTYmNjGfWYAaKioh6a2syXq7RLOWbHjh17aHvKayPHNO1SjllKqc/0+8cXERGh8PBwrVixQjt27LB1nCcOz82Mdfv2bSUkJNg6Rrb37rvv6tChQ7aOka2l/G1/8803unPnDp858cSy2RpSTzIHBwd5e3vL29tbUVFROnv2rPbt2ycvLy/dv39fYWFhmjBhgq1jZispL8Lh4eE6c+aMSpYsqZo1a8rZ2ZkPY38jd+7cevXVV7V7925t2rRJO3fuVJEiRVSjRg35+vrKy8vL1hGznZRpt7t379bdu3d1+PBhNW7c2NaxsrXp06drzZo11pLP3d2dv+fHYGdnpxs3bmjSpEn64osvlD9/fkn//3WTY5p2Kcds3Lhx2rFjh2rWrKm2bduqRo0aypEjh43TZS/37t3Tt99+q/Xr16tly5by8fFRwYIF5ezsrKtXrypv3rzKmTOnrWNmCylrkz548EDHjh3TokWL1Lp1a/n5+dk6WrZlsVjk4OCgX375RStWrFDRokXl7e2tMmXKqESJEvL09OQ1NA1Szoz+0ksvae7cuSpfvrxy5MihEydO6NixY+rcubNcXV1tnDLrS/nMeerUKd27d++hy1JGoXEWejwpWEMqE0VHR8vNzU0JCQnau3evDh48qOvXr6t+/frq0qWL9U0QqRMXF6dffvlFJ0+e1P3792Vvby8fHx/Vrl2b043+g2HDhqlu3boyDEORkZHatm2bkpOTNWDAANWvX9/W8bKl7du364cfflBYWJiqVaumli1bqlatWsqdO7eto2ULKR+ydu3apV9++UVvvPGGhg0bpgULFujzzz9XYGCgypYta+uY2dKXX34pLy8vdenSRRcvXtSJEycUHByst956y9bRspWUL/0HDx7UlClT9N5772n58uXauXOnnnnmGdWpU0fvvPOOnJycbB0124iKitKECRN0//59HT58WEWLFlVAQIAWLVqkiRMnqkyZMraOmC2kvH5Onz5d9+7d0/Xr1yVJY8aM0aZNm9SyZUvKk8f02muvqX79+kpOTtbFixeVmJgoFxcXdejQQdWrV7d1vGzh66+/VkxMjNq1a6dKlSrpq6++kr29vXbu3Kn8+fPLyclJX3/9ta1jZitLly7ViBEjVLBgQQUFBalHjx5yd3e3dSwgQzFCKoOlfJA9efKkFixYoOPHj6thw4bq0qWLnn/++YeuSxmVOinH9JlnnpG/v78qVqyoO3fu6Pr16zp27Jju3r1LIfUnKcfryJEjunHjhjp27Cjpjy8EefPm1aFDh564M1qaqXHjxqpXr55iY2P1008/6bvvvtOIESM0b948vlSlQsqXpQ0bNqhVq1bat2+f6tatK0kqUaKENm3aRCGVSgkJCRo8eLACAgLUoEEDtWnTRlOmTNGCBQtUrFgxJScnq2fPnraOme2kvIaeP39ebdu2lY+Pj4YPHy5J2rp1q06cOEEZlUopBUpSUpK6du2qihUrKiYmRjt37tTGjRvVsGFDXjfTIGXU42+//aYxY8ZoxowZ8vX1lbOzsw4fPmwd2YPUSflbDw8PV6FChfTiiy9K+uO19fDhw9qxY4c8PDxsnDL78Pb21t69ezVu3DjlzJlTN27c0DPPPKORI0fyOf0xBQYGKjAwUDt37tS0adM0efJkFS5cWNOnT2e2A54YFFIZLCkpSU5OTpo1a5aKFy+ukSNHauXKlXrttdeUnJysN998U+3bt7d1zGwl5QvshAkTdPz4ceXJk0f//e9/ZW9vz5Spv5FyvHLnzq24uDjNnDlTHTp0UN68eVWxYkUdOHCA6RFplDKacdu2bTp+/LjWrl2rvn37atCgQRo0aJCOHz/Ol4BUSnl+Vq9eXaGhodq8ebO+/PJLSX+sgZTyN82ZSf9dcnKySpcurdmzZ2vKlCmqX7++4uLiVLFiRQ0dOpS/88eU8ry7cuWKTpw4oeTkZNWoUUNlypTR888//5cfl/DPUo7l8OHD1apVK5UsWVJnz56VxWLRhAkTrFNPkHp37txR/vz55eDgoMuXL2vYsGGSpBMnTqhHjx42Tpe9pLwfnThxQps3b5ZhGOrZs6e8vb1Vt25d648lSJ3mzZurUaNGCg4O1sWLF3Xo0CFt2LBBs2fPVr169dShQwdG8KVCyuefq1ev6tixYzp9+rRKlSqlKVOmyNHRUbNmzaIoxROFQioDRUZGauvWrapQoYLy5cunoKAg5c2bV7Vq1VJ0dLQ2bNigokWLSuLLVmqlHKd169YpISFBb731lr766iu5uLhowoQJateuHaMp/iQmJkaHDx9Wo0aNVKpUKb3zzjtauHChNm3aJMMw5OzsrHbt2tk6ZraTMppxyZIl6tWrl4KDg5UvXz7rF9Z27dpZf2nFP/vzMWrXrp0GDBigXbt2acKECcqRI4euXbumgIAASeL1MRVcXFw0ePBgSdKFCxe0fv16HTlyRKGhofr+++/VsWNHitI0unDhgsqWLauEhATVq1dPOXLk0NGjR3XixAkVKlRI3t7eatasma1jZgsp79+HDh2Sq6ur2rVrpzVr1mjBggUqU6aMkpOTeT9KI8MwlC9fPpUvX15NmzZV8eLFde/ePa1bt065cuVS6dKlbR0xWypXrpzeeust7d+/X59++qly5cqlypUrq1evXnJzc+O9PRVSfrj7/fffdfbsWZUoUUJNmzZV+/btdfToUV24cIHjmEbTpk2TxWJR2bJldeHCBW3fvl1vvPGGXn/9dU5WgicKhVQGunTpkubPn29dS+ann35S586dlT9/fuXMmVOdO3e2XpcvW6mT8ub122+/KSAgQMHBwWrQoIEkyd3dnek9/+PSpUtycXHRlStXNG/ePDVs2FAvvfSSHB0ddfHiRXl6eqpWrVq2jpktBQcHKz4+XvXq1dM333yjevXqKTExUUuXLlWtWrVUuHBhW0fMNr788ktVrlxZ33zzja5fv66ff/5ZhQoVUo8ePWRvb09hnwaJiYk6d+6cQkJC1LZtW7355ps6ceKEfvjhB124cIFCKo3mzJmjgQMHavXq1apSpYrefvttRURE6MCBA9q7dy9rxaVByt/wjh07VL58eS1dulSnT5/WsGHDlJCQoNmzZ1NIpZGdnZ1+++039e7dW5UqVdL8+fPVunVrBQQEqG/fvpLE+qSplPIDicViUb58+RQYGKjWrVvr6tWrOnz4sE6dOqWEhATW60klBwcHJScn66OPPlLbtm3l7e0tV1dXnThxQnXr1uW9KA3s7e0VGRmpM2fOaMmSJUpKStKdO3e0fv16zZ49W++//77y5Mlj65hAhqGQykA1a9bU0qVLdenSJW3btk3bt2/XmTNnVKVKFVWtWlWVK1fmw2wa2dnZyTAM1apVS3v37tWuXbs0btw4SdLp06f5MPs/qlatqsTERF24cEGStHHjRjk5Oalo0aKqUqWKKleuzBf9x2AYhtzd3VWqVClNmDBBPj4+ypEjh86ePStXV1fKqFSys7NTXFycYmJiNG7cOE2bNk01atRQ+/btVbZsWeuXKJ6j/y6ltFu/fr2+/fZb+fr6au3atcqRI4fq1q2rTz75hA+saZSQkKCPPvpIDg4OioiI0IABAyRJHTt2VK9evdSqVSvFxcXZOGX207x5c33zzTeKjo7WoEGDVKlSJY0cOZKRZmmQUp5cu3ZNU6dO1dKlS1W1alUNGTJERYoUeei6lFGpk5ycLAcHBy1cuFA///yz7t27p06dOql9+/YqXbq08ufPr3z58tk6ZraQ8vzcvHmzvLy8FBQUpMTERFksFjk7O2vbtm3y8fGxdcxsJSIiQoUKFVJsbKxy5MghDw8PtWvXTlu2bOG9HU8cCqkMkvJifO/ePa1du1aBgYF6+eWXdeTIEa1du1Zjx47VF198QSGVBjExMXJ3d1dkZKSqVKmiI0eOKCkpSatXr9b58+eVnJyspk2b2jpmlvHn00FbLBaNGDFC4eHh2rt3r86ePauZM2fqnXfe4Veqx2BnZyd3d3eVLVtW06ZNU44cOTRq1ChFRkYy4iyVUn61X7p0qfLly6f33ntPbm5uWr16tQYNGqTChQurffv21kX48Wgppd2lS5f09ttvq06dOjp58qSuXLmiHTt26ObNm3rllVdsnDJ7WbdunQ4cOKBq1appwIABGjZsmE6fPq1Zs2apWbNmKl++vFasWGHrmNlOxYoV9frrrytfvnwqWLCgpk+fruvXr1NIpcH/fuG3WCy6evWqhg8frhIlSqhKlSry9/dnNE8apIzoWbZsmebNm6cuXbpoy5YtmjJlikqUKKH+/fvbOmK2kTKbwc3NTblz51ZiYqL1xA8po6SQOrdu3VKBAgVUrlw5FS1aVC+99JIaNmwoHx8fnTt3js/weCLZGUxCzRApv1afPn1aI0aMUGJioooUKaKAgAC1aNFCTk5OcnZ2tnXMbOX48eM6dOiQdu3apTfeeEO+vr7av3+/Ll68qJIlS8rHx4dfr/7G3r171adPH3l4eKhjx47q0aOHChUqpIsXL+rZZ5+1dbxs5fbt2zpy5Iju3r2r8+fPa/jw4QoPD9ehQ4e0f/9+tWrVStWqVeNvOw26d++u//73vypWrJgSEhIUERGhuXPnqkCBAgoODtarr75qXWsPjxYdHa0vv/xSgYGBqlixoiQpPj5eV69eVYECBXh9TKNdu3bpxIkTunr1qm7cuKHKlSurVq1aeu655+Tg4KDz58+rXLlyto6ZLaR8JlqzZo3WrFmjpKQkvfvuuypTpowuXrwoFxcXFStWzNYxs5X4+Hh16dJFq1evlsVi0e+//67Fixfr1q1bcnJykp+fn1q0aMF6hqmQcoy2bdumjRs36u2339ZHH32kqVOnatmyZYqOjlZQUBCjzdIoOTlZH3zwgbZt26bmzZvL19dXS5cu1WuvvabnnnvO1vGyvPPnz+vSpUtq2rSpTpw4oVKlSunw4cO6ePGidu/erbp166pLly4saI4nDvMiMkjKr9Vz5sxR9+7d9eabbyogIEDz5s1Tz549NXr0aF26dMnGKbMXLy8v3b9/X/v27dOvv/6qmTNnKkeOHOrRo4fCw8OVI0cOW0fMkurVq6ezZ89q3LhxOnv2rJo2bapWrVrpwYMHto6W7bi4uCg0NFSfffaZFixYoO+++04Wi0WtWrXSiBEjVLBgQcqoNEhMTJSvr6/Gjx+vs2fPytnZWUWLFtXp06fVoUMHhYeHKzQ01NYxs40LFy5o+fLl6tGjh0aNGqXLly/LxcVF5cqVo4x6DA0aNFC7du2UmJioMmXKKCEhQatWrdIbb7yhSZMmcYrtNLC3t9edO3c0e/ZsDR061LqG4U8//aS4uDjKqMcQHBysvHnzKiwsTA4ODipTpozef/99SZK/v7/mzJmj6OhoyqhUSDlGKQvBL1myxDq6LGURc8qo1PnzuIaIiAiNGjVKS5cuVd68eXX48GENHDiQMiqVXF1dVaNGDf3222/68ccfNW/ePMXExKhmzZr68ccfNWDAAMooPJGYspcBUn5puXjxos6dO6fPP/9ckhQbGys3NzcdP35chmFo+/btKl26NB8WUilv3rxq06aNSpQoIQcHBx04cEBnz57VvXv3dPXqVab2/I24uDjdvHlTXl5eqlevnurVq6dDhw7pxx9/lIuLi63jZTtubm7q3bu3LBaLvLy8tGTJEk2ePFmlS5fW/fv39cYbb6hUqVK2jpktGIYhJycnvfjii5o6darGjh2rqKgolSxZUi4uLnrmmWd0+/Zt1a5d29ZRswXDMFSjRg0dO3ZM58+f18yZMxUYGCjDMDR58mTryR+QOilTSpcsWaLq1aurZ8+eio2N1alTp/T999/LMAy5urraOma2kDI6avPmzWrUqJHs7OxUqVIlubm5qXTp0lq+fLkqV65s65jZjre3t3x9fTVo0CDVqlVL3t7eCg4OVrFixVShQgXlyZNHOXPmtHXMbKVGjRoqV66cYmNj9eWXX2rcuHHavHmztejDv0v5TjNx4kSFhIRo165d8vHx0YABA3g/T6OUHz3Onz+vjh076tSpU9q9e7dcXV21ZcsWdenShc+ceCJRSGWAlBdjFxcXubm5aeHCherQoYNy5MghHx8fbd26Vf369dOIESOsZ0FB6iQkJChHjhyqV6+eWrVqpRMnTigsLEyFChWydbQsJaUU3b59u/bt26cqVarIy8tLFStWVK5cuVS2bFnmnadRypeq6OhotWrVSs7OzmrevLmSk5P1888/Kzw8nEX108DOzk5RUVFKSkrSq6++qrt37+rGjRuKjo6Wu7u75s+fL39/f1vHzPL+vF7hnj17dPLkSeXJk0dvvPGGPv/8cy1ZsoQpj48hZTSEk5OTDh06pMaNG6tYsWKqVauWTpw4obx589o4YfaRMmI8Z86cioqK0qRJkxQQECDpj1E+jDxJu9jYWB0/flzdunVT5cqVdeXKFa1atUoFCxZUrVq1NGXKFDVq1MjWMbOFlPL50qVLOnr0qCpUqKBy5cqpffv2OnbsmIYOHarnn3/e1jGzhZT3o+DgYB09elQTJkxQjhw5tHz5ck2ePFnvvvuuqlSpYuuY2ULKZ86jR49q06ZNGjVqlPz9/RUWFqb9+/fr4MGDjHzGE4s1pNIpISFBBw4csA5H3blzp+bOnav79+/rmWeekaOjo5o1ayY3NzcdOXJEH3zwgY0TZ30pL8oHDx7U+PHj5ebmpitXrqhChQrq0qWLmjRpwiizf/DLL7/o/Pnz1iH9+fPn1549e9S0aVPrGaOQOinPwyFDhujSpUsqVqyYSpcurcqVK6tKlSqUoqn057/nyZMnyzAMlSxZUlWrVlXFihV19OhRdevWTTdv3lSuXLkYhfIvUr5MTZs2TSdOnJCvr6/u3r2rM2fOqG3btmrVqhVryDyGlGN28+ZNTZw4UbGxscqdO7cKFSqkzZs365tvvpGnp6etY2Z5YWFhypcvn3Uq88cff6y1a9eqZ8+ecnBw0I4dO/Tpp5+qbNmyNk6avWzbtk1z5sxRxYoVVbx4cRUpUsS6jub58+d18eJFNW/e3LqQNP5d//79FRUVpeDgYJUqVUodOnRQrVq1GIGSBinvR99//71iYmI0ZMgQJSUlydHRUStXrtS+ffuss0bwaCnvQStWrNCMGTM0cOBA1atXj1GPeCpQSKXTqVOndOvWLfn4+Oinn35S48aN5erqqsTERJ04cULFihVTfHy89uzZo6CgIJUvX97WkbO8lBfliRMnysPDQz179tS1a9e0du1aLV++XKVKldK3335r65hZRsoX/uPHj+vYsWMKCgpSZGSkDhw4oIsXL6pcuXKqW7cuZ995DFFRURoyZIjGjRunI0eO6PDhwwoLC9ODBw80bNgw1pRJhZTn5zvvvKPOnTtr8+bNunz5suLi4hQTE6NKlSrxgfUxBAYGatasWdYzke7fv1+rV6/W22+/zWjINEp5z0l5rt65c0eHDx9WaGiorl69qurVq6tNmza2jpktzJgxQ76+vgoLC5OdnZ1atGih06dPa/Xq1cqdO7dq1qypmjVr2jpmtpOcnKx9+/bp8OHDCgkJ0Y0bN1SqVCl169ZNPj4+to6X7dy4cUOjRo3Sd999J0latWqVfv75Zx0+fFirVq1S8eLFbZwwezl+/Li+//579e3bV76+vpL+mMKXL18+9e7d28bpspfVq1fryJEjunnzplxdXVWmTBlVrVpV9erVs3U0INNQSKWTxWKRxWLRqVOntGLFClksFrm6uqpYsWKqXr26KlSooAcPHigyMpIvr2k0ffp0lShRQs8///xDQ/zv3LnDsNU/Sfk1atq0aTp06JAmTpzIelHp9Oc1UA4cOKD33nvPellISIiOHj3KF9Q0sFgsevXVVzVt2jS98sormjhxoiTpxx9/VO/evZUvXz7rL634Zyl/6/fu3dPo0aP1+uuvP3TmzKCgIE2aNEn58+e3YcrsKTk5WZ999pnOnz+vGjVqqHbt2qpatarOnj2ratWqydGRFQ7SYuXKldYv+/7+/urcubP1Sz4j+FIn5TjFx8c/9J5+9+5dLV++3Dr6JF++fBzTVEp5b79x44ZmzJihZs2aqU6dOtbLo6KilCtXLhsmzD6OHj2qCxcuqHHjxvLw8ND06dM1b948SVKdOnV08+ZNjRkzhtHkqZDyvExZE7Jt27Y6efKkgoODdf78eUVERGjcuHGMgMQTi09Y6eTg4CAHBwdVq1ZN1atX17Vr17Rnzx5dvHhRv/32m958801VqlSJ0SlpdPr0aS1atEgFChTQ7du3VblyZRUuXFi5cuWijPofjo6Oio6OVt68eRUTE6O33npLZcuWVZ06dVS7dm3OAvcYUtZACQsL04oVK3ThwgW1b99efn5+KlasGGeISqV9+/bJ1dVV7u7uqlmzpubNm6dcuXLp3r178vT01Llz56xr81BG/buxY8eqXLlyqlq1qgoXLqy3335b9erVU9myZWVnZydXV1fKqDRK+SKwZs0aJScnq3Xr1vrqq6+0Y8cOSdKDBw+0fPlyCqlUSClFzpw5o5w5c2rdunU6ePCgVq1apX79+skwDK1YsYLPQ6mUUjAtXLhQ69atU0BAgJo2bSovLy916NBBFy5csH4eooxKnZT39rffftt6spzChQurZs2aatKkicqUKWN9TcCj/f7779q9e7f27dsnLy8vtWjRQl27dtWVK1d07do1NWzYkHIvjX7++Wf5+vrKxcVFNWvWVNWqVRUaGqr4+HjKKDzRGCGVDim/6P/222+aNWuWLl68qO7duyswMFC5c+fW6dOnVb58eT4opMGffxFMTk7Wrl279Msvv+jevXsqWLCgXnjhBYb7/8mVK1e0ceNGrVixQm5ubmrQoIHy5MkjJycnnTx5UhaLRZ9//jlf9h9DQkKCQkJCFB0drcOHD+vw4cOKjIxU4cKF9fHHH8vNzc3WEbO8li1b6sGDB+rXr5+8vLyUO3dubdiwQdu3b9czzzyjatWqacSIEXwBSIX4+Hj16tVLUVFRatmypYoVK6Y8efLo/v37Wr58uby9vfXCCy8wXS+NUt5z3n//ffXu3VvHjh2Ti4uL/P39NWbMGLVt21a1atWydcxsITExUU5OTlq+fLni4+PVo0cP62XR0dE6c+YMZ916DJcuXdLBgwd16tQp/f7773rmmWcUHR2tNm3aqFevXrx+ptKfC9OpU6dqypQpOn/+vI4dO6ZDhw7p0qVL+vHHH5UnTx5bR80WYmJidO3aNZ0/f16XL1/WtWvXZGdnp1q1aqlSpUqqVKmSrSNmKwkJCerfv7+OHDmijh07qkePHipXrpytYwGmoJBKh5Q3t759+6pNmzbKmTOnZs2apePHj6tIkSIaO3asqlevbuuY2U5sbKyCgoLk7e2ttm3bqk6dOoqIiNDy5cv13HPPccaOP/nPf/6j0qVLq02bNrp796727Nmj1atXy8fHR+3atZOrqyunf0+jlA/3K1eu1JUrV9SgQQMVKlRIdnZ2unz5soKDg/Xiiy/aOma2cOzYMY0dO1ZRUVGqUKGC3Nzc5OrqqsqVK+v+/fuqV6+eihUrxheqVLp06ZI+//xzhYSEqHbt2kpKSpKrq6tKly6tcuXKUZykw/fff69cuXJp165devHFF1WnTh2NHTtWHTp0YI2eNIiJidHLL7+sAgUKqHfv3vL19eUHkceQ8vkyKSlJsbGxun79uqKjo+Xg4KCTJ08qLi5OQUFBypEjB9P1UunPoyEPHDigvn37ytPTU05OToqKilJ4eDiL7adSyrE8deqUTp8+rZYtW+rs2bMKDg7WmTNndPv2bY0fP55RPWn04MED7d+/X2vWrNGhQ4fk7Oyszp07q0+fPraOBmQqCqnHlPIBICYmRuPGjdMnn3xivSwhIUHTp0+3lid8WEibBw8eWBfoPnjwoKKiolSnTh21adOGX///5OzZs/rvf/+r6dOnP7T97t27Gj58uAYOHMgi+umwZcsW/fLLL7p165Y8PT1VoUIFVapUSc8++yy/oKbBuXPntGTJEpUqVUq+vr46f/68duzYoeLFi+s///mPreNlO4ZhaMGCBTIMQ+3bt1d4eLiWLVumIkWKqFevXraOl60cOXJETk5OevbZZ/XMM8/ozp072r9/v+bPn69y5cppz549Wrt2ra1jZgtHjhzRoUOHdPLkSV27dk0FCxbUxYsX5enpKT8/PzVv3px1NNMg5Qv/rFmztGXLFuXJk0dFixaVj4+P2rdvb+t42dro0aN14cIFeXl5qVq1anr22WdVvHhxFShQwNbRso2U5+fo0aNVs2ZNtWrVStIfoyRTpphR5KfNpUuX9ODBAxUqVEi5cuVSfHy8Nm/erOTkZHXq1MnW8YBMRSH1GP5cMO3YsUOzZ8+Wt7e3AgICVLRoUdY4yiAJCQmKjIzU+vXrtWbNGrVo0UJ9+/a1daws4+uvv7aOjkpISLBud3Z21sKFCxUcHKxhw4bZMGH283cjdSIiIrRu3TrNnDlTzz77rCZNmqQcOXLYKGH2dOPGDU2YMEHOzs56++23lTdvXl2/fl3FixdndNRjiIqK0tdff63Dhw9r5MiRqlatmnXBc6Te4MGDFR4eLh8fH+s0EwcHB23cuFGSVKxYMfn5+dk4ZfbwyiuvqGrVqvLx8dGBAwcUEBCg6tWra+XKlZo7d64qVaqkjz/+2NYxs5X4+HgFBQXp+++/17Vr13T27FmtWLFCHTt2VNeuXfmhMx1u3rypzZs369ixY4qPj1epUqU0cOBA3ovSgClmGSc4OFgff/yxbty4oZw5c6p+/fpq0KCBVq9ercGDB/MjKJ54FFKP6erVqypevLgOHDigXbt2KSQkRDly5FCxYsVUpEgR1alTRx4eHraOme2EhYVp69atat68+UO/Vo0bN059+/ZVwYIFbZgua6levbo6deqkN9544y8LGc+aNUsRERF69913bZQue1u2bJkMw9Dzzz9vPbaHDh3S9u3bNXjwYBuny/ri4+N1//595c+fX7dv31ZCQoLy58+v0aNH6969exo1ahTFfRqkrM9RqFAhxcTEKCQkRJUqVdLixYu1d+9effjhh6zN85hOnjypTZs26dixY7Kzs5Ovr69q1KihYsWKMaInlc6ePasvv/xSP/zwgwzD0N69e7Vs2TKNGzfOWpImJCRwgo1USvnRc8uWLVq9erX1rKTSH8f622+/1VdffWXDhNlPyg8f+/fv14EDB5QnTx75+fmpcOHCWrt2raKjo9W1a1dbx8x2mGKWPinr7o0bN05VqlSRu7u7Zs2aJTc3Nx0/flzNmjXTiBEjbB0TyHT8nPoYDh48qMWLF2v8+PGqVauWatWqpZs3b+q3337TyZMndfToUdWrV8/WMbOV6Oho5cyZU3fv3tWcOXP0008/qXLlymrTpo3u37+vvXv3MtrnTywWiz777DNt2LBBgYGBKly4sNq2bat27drJzc1NR48e1euvv27rmNlKeHi4ZsyYod69e0v6owTYt2+fChUqpAYNGmjZsmV6/vnnbZwyexg1apSOHj2q3Llz67nnntPJkycVGhqqypUra8eOHRoyZIhmzpxp65jZRrdu3fTgwQMVKFBAHTt2VGxsrBYvXiwfHx+5ublp7969FFJplHJSkj8vvnvkyBFt2LBBEyZMkK+vr95//30bp8weNmzYoLZt20r642xv9vb2slgscnR0VEJCghwdHSmj0iBl5FPlypW1cuVKTZ8+XY0aNVLZsmV14cIF6wk1GF2aevb29rpz547GjBmjrl27avr06fr1119VtGhRRUdH80PTY0iZYlahQgXVrVv3oSlm+HcJCQlasGCBevfurdjYWD377LP68ccfNXz4cJUpU0ZTp05V06ZNbR0TMAWF1GPw8PBQWFiYjh8/bl1g28PDQ+3atVOzZs109epV5qKnQVJSkr7++msVLVpUTZo00Zo1axQaGqqVK1dqwoQJKl68uF5++WVbx8xSHBwc1KpVK7Vq1UoRERHatGmT1q5dq2nTpilPnjyyt7eXt7e3rWNmKw8ePNC+ffu0cOFCubi4qFmzZtaFo5ctW6aQkBA+HKSCxWKRvb29ChQooLt37+rKlSt6//33lTt3bsXFxemzzz7T3bt3rddlweNHS05O1scff6yLFy/qzJkzOnnypHr16qV3332XL6PpkPK8mzJlivX5WL9+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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABKQAAAIqCAYAAAAaSZJCAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAAC3eklEQVR4nOzdd3iN9//H8Vem2Dtib7FXFLXShkbsvVeMqlmqLaXVr93Soa2t1KpRStXexGwIsfeIiC1EEiHj5Pz+8D3nR1uq/dZ9Hzwf1+W65Kz7fe5zz9f9+XxuJ6vVahUAAAAAAABgEGezCwAAAAAAAMCrhUAKAAAAAAAAhiKQAgAAAAAAgKEIpAAAAAAAAGAoAikAAAAAAAAYikAKAAAAAAAAhiKQAgC88qxWq2bNmqWAgADVrFlTtWrV0rBhwxQbG2t2ac9kzZo1f1prRESEvL29FRAQoICAANWuXVv+/v4aO3asLBaLCZX+7xYvXvy3X9epUycdO3bsX5n+hAkT9PHHH/9Pn7Fq1So1adJEAQEBqlWrlnr16qXr16//K/UBAAC8KAikAACvvC+//FJr1qzRrFmztHnzZq1YsUKJiYnq3r27rFar2eX9pe++++6J4ZmLi4vWrVundevWaf369Vq2bJn279+vpUuXGlzl/+7mzZuaMWPGX77OYrFo3Lhx9r/nzJmjEiVKPM/SntnZs2c1ZswYTZgwwf6b5M6dW0OGDDG7NAAAAEMRSAEAXmlRUVGaN2+ePv/8c2XPnl2SlCpVKn366afq1q2brFar4uPj9emnn6p27dqqU6eOPv/8c1ksFo0dO1ajRo2yf9adO3dUtmxZxcTE6OzZs2rfvr1q166tBg0a6MiRI5Kk4OBgtWrVSl999ZXq1KkjPz8/7d27V5J0//599e/fX7Vr15afn5/Gjh1r/+wOHTpo1qxZatOmjapXr64BAwbIarVq8ODBunDhgjp06KCQkJC//L5p0qRRpUqVdOLECUlSTEyMPvzwQ9WuXVs1a9a0B1URERHy8fHRjBkzVL9+ffn7+2vTpk2SpGXLlqlPnz7q1KmTPfhZvHixAgIC5OfnpwEDBujBgweSpL1796pJkyaqW7eu6tSpo7Vr1z51upLk7e2t5cuXq3HjxqpWrZpmz54tSWrdurWuXLmigIAAJSQkKDQ0VE2bNlVAQIDq1q2r3bt3S5I6d+6smJgYBQQE6NKlS/Lz87PPm7Vr16p+/foKCAhQx44dFR4eLulhy6cRI0aod+/eqlmzppo3b64bN2786Ty8d++e3nnnHfn5+alDhw66deuWfvzxR73zzjv21yQnJ6tKlSo6efLkY+89c+aMMmfOrFy5ckl6GBi+9957+vLLLyVJH330kT777DN16NBBfn5+evfdd3X//n1JeuIyJUnTp09XzZo1Vbt2bX322WcvRJAKAABecVYAAF5h27Zts7711ltPfc20adOsb7/9tjUxMdF6//59a7NmzazLly+3Hjx40Prmm2/aX/fzzz9b33nnHavFYrHWr1/funjxYqvVarWGhIRYq1WrZk1MTLT+9ttv1pIlS1o3btxotVqt1u+//94aGBhotVqt1pkzZ1q7detmTU5OtkZFRVkrVqxo3bdvn9VqtVrbt29vbd++vfX+/fvWe/fuWV9//XVrSEiI1Wq1WosUKWK9evXqH+q+dOmStVixYo89du3aNWtAQID1119/tVqtVuvw4cOtAwcOtFosFmtkZKTV19fXeurUKeulS5es3t7e1hkzZlitVqt1165d1kqVKlkTExOtS5cutZYtW9Z64cIFq9VqtR46dMhapUoV67Vr16xWq9U6dOhQ6+eff261Wq3Wpk2bWoODg61Wq9V64cIF64ABA546Xdv3+eKLL+yfXapUKWtSUpL1t99+s9aqVcv+XerXr29dtWqV1Wq1Wn/55Rf7c7//3m+++aZ137591suXL1t9fHysYWFh9vndqVMnq9VqtX733XfW119/3RoREWFNTk62du/e3Tp58uQ/zNPvvvvOWq5cOWt4eLjVarVa33//fevo0aOtt27dspYuXdp6+/Ztq9Vqte7bt89au3btP7z/2rVrVh8fH+s777xj3bhxo/XOnTuPPT9o0CDrm2++ab19+7bVYrFY27VrZ509e/ZTl6l9+/ZZ33rrLWtMTIw1Pj7e2qxZM+uaNWv+MG0AAABHQgspAMArLSYmRpkzZ37qa7Zt26aWLVvK1dVVHh4eatCggXbt2qUyZcrIarXaW8Fs3LhRderU0fnz5xUeHq5mzZpJknx8fJQpUyaFhoZKklKnTq1atWpJkkqUKKErV65Ikrp06aLJkyfLyclJ6dOnV+HChRUREWGvIyAgQB4eHkqVKpXy5cunq1ev/uX3s1gs9jGk3njjDTVt2lTt2rVTw4YNJT1sMdS6dWs5OzsrU6ZMeuutt7RhwwZJD8fWat68uSSpSpUqSkpK0sWLFyVJ+fLlU758+SRJ69atU82aNZUtWzZJUps2beyfkTlzZi1fvlznzp1Tvnz59NVXX/3ldCWpUaNG9vkTHx+vyMjIP3y35cuXq06dOvZ5fOnSpafOi127dqlSpUrKmzevJKlFixYKDg5WYmKiJKlChQrKmTOnnJycVKxYsSfOXx8fH+XOnVvSw9/k4MGDypw5sypUqKD169dLergs1K1b9w/vzZYtm5YsWSJPT0+NHDlSr7/+ugIDAx9rSeXn56eMGTPK2dlZtWrVUmho6FOXqe3bt8vX11dp0qSRu7u75s2bJ39//6fOCwAAALO5ml0AAABm8vLy+ssBpW/fvq306dPb/06fPr09IHnrrbe0efNm5cmTRwcOHNCXX36p06dPy2KxPBZIxMbGKioqSunSpVPatGntjzs7Oys5OVmSFBYWps8//1znz5+Xs7Ozrl27pqZNm9pfmyZNGvv/XVxcnmlgctsYUpJ07tw5tW3bVvXq1bM/HxMTo4EDB8rFxUWSFB8fr4CAAEmyB2M26dKl0927d+3z4NHP2Lhxo73rodVqtYc8Y8aM0ZQpU9S5c2d5eHhowIABCggIeOp0Jdnnke152zx61MqVKzV37lzdu3dPycnJf9lN7c6dO0qXLt1j07BarYqKinpsmrbpPmn+ZsqU6bHPsM2TevXqadmyZWrdurU2b96sKVOm/On78+fPrxEjRkh6+JtMnz5d3bt317Zt2yRJGTJksL82Xbp0io6OVnR09BOXqTt37sjT09P+eMqUKZ86HwAAABwBgRQA4JVWtGhRRUdH6+jRoypZsqT98cTERE2cOFE9evRQlixZ7KGF9HDcqSxZskiSateurTFjxqhw4cJ67bXXlCZNGnl6eip16tT2IOhRwcHBT6xlxIgRKlGihCZNmiQXFxe1bt363/uikgoWLKg333xTkyZN0ieffCJJ8vT01KRJk1SkSJHHXhsRESGr1ao7d+4oY8aMkqS7d+8+FkTZeHp6qkmTJho0aNAfnsuSJYuGDh2qoUOHaufOnerbt6+qV6/+xOk+q+vXr+uTTz7RkiVLVKxYMYWFhal27dpPfU/mzJntrdRs38fZ2dn+/Z6VLYCSpOjoaHuA5O/vrxEjRigoKEgpU6ZU4cKF//De48ePy8PDQwUKFJD08DcZOnSofHx87J97586dx6aVPn36py5TR44ceew9tv//3e8FAABgJLrsAQBeaWnSpFH37t310Ucf2buj3b9/X59++qmOHz+ulClTytfXVz///LMsFovi4uL066+/ytfXV5JUvnx5RUZGatmyZfbuYzlz5pSXl5c9PLh9+7YGDBiguLi4p9YSGRmpYsWKycXFRbt27dLFixd17969v/wOrq6uio6Ofqbv26dPHy1dutT+Xf38/LRo0SJJUlJSksaMGaNjx47ZX79q1SpJ0s6dO+Xh4aH8+fP/4TP9/Py0YcMG3b59W5K0adMmTZ8+XYmJierQoYN9cPASJUrI1dVVLi4ufzndJ33PuLg4JSUl6fbt20qVKpXy58+vpKQk/fTTT5Iethpyc3NTcnLyH+48WLVqVYWEhNi79i1atEhVq1aVq+vfuz63f/9+ezfLdevWycfHR9LDZal69eoaPny4fVn4vZ07d2rQoEG6deuWpIetyVauXKlChQrZA6QdO3bYW0Rt2rTJ3pXwScuUn5+ftmzZort37yopKUm9e/fWzp07/9Z3AgAAMBotpAAAr7zu3bvLw8NDPXv2lMVisQcmw4YNkyR17NhRERERqlevnpycnBQQEGAPHJycnFSrVi0tWbLEPj6Sk5OTvv76aw0bNkzffPONnJ2d1blzZ6VKleqpdfTs2VOjRo3SxIkT9dZbb6lPnz76+uuvVbx48ae+LyAgQK1bt9aoUaP+dNyiR+XKlUtNmzbVl19+qQkTJqh///4aPny4vXVR9erVVbRoUV29elUuLi5KTExUvXr1FB8fr1GjRsnZ+Y/XskqUKKEePXqoQ4cOSk5OVubMmTV8+HC5ubmpefPmCgwMlPSwe+Inn3wiDw+PJ073aby9vZU+fXpVrVpVy5YtU40aNeTn56fs2bPro48+0oEDB9S2bVstX75cPj4+evPNNzVt2jT7+728vDRy5Ej16tVLSUlJypkzp0aOHPnUaf4ZPz8/jRw5UqdPn1auXLn08ccf25+rV6+eNmzY8MRA6u2331ZycrI6duwoi8WipKQklShRQlOnTrW/pnLlyurTp4/Cw8NVunRpNWvW7KnLVNmyZdW1a1c1btxY7u7uql69uurXr/+3vxcAAICRnKx/NeACAAB45URERMjf31/Hjx83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detWTZ48WaVLl1avXr3k6enpcOu8zeHDhxUaGqrTp08rXbp0GjRokNkl/UFwcLC++uorBQQEqF27dkqRIoXDjtG0b98+BQYGqmzZsgoMDFSlSpWULl06s8vCK8S0u+yZxdYC4tSpUxo6dKj9JHn58uX69ttvdeXKFf3nP/8xs0RJ0oEDB1S4cGFFRUXZT1TSpUunWbNmKTAw0LS6bBvT0NBQZcyYUb6+vho7dqwyZ86sChUqaO7cuSpfvrzDnpBK/3+VL02aNCpdurQkqVq1aqpWrZpu376tmzdvmlLXo1dW6tSpo+LFi8vHx0dOTk6KiorSL7/8or59+5pS219xcnLS7du3NWTIEJUoUUKhoaHy9vaWr6+vDhw4oJ49e+qrr75SyZIlTa3T1nXL29vb3lXq6NGj6tatm9577z35+PiYesDg5OSkuLg4pUiRQj179pQkffjhhwoJCdHs2bN169YtU08ObNcv5syZo4sXL+rkyZOqUqWK6tevryJFiig0NNRh132LxaI8efKoYMGCypQpk6pXr65z587p4sWLKlGihGE1uLi4KCIiQocPH1bGjBn17rvvysnJSUuWLFFMTIypYZQk+8nHyZMn1blzZ23evFlvvPGGpIf1Hzx40KECqR9++EH37t1Tnz59FBgYqKlTp6pgwYLq16+fKlSo4FAtJWxs25gWLVpo+fLlOn78uHr06KFz584pJCREn3zyieE1PXri6e7urvr168vf319r1qzRxo0b1bx5c4c5MbXNv23btqlQoUIqWbKkkpKSJElVq1bV8uXLX5hA6tq1a3J1ddWtW7eUKVMmVa1aVZGRkdq3b59atWplSCBg2y7ZhofIli2bIiMjdfr0ae3evVulSpXSu++++1xr+Cds8yU6OlqDBw9WmTJldO3aNV24cEGbN2/W6dOnTQukbPN0w4YN2rdvn4oWLar27dsrX758+vHHH/XgwQO1a9fOlNpsHj3WcXFxUa1atfTGG29ow4YNCgoKUosWLRxmnZekRYsW6ZdfflHlypXVrFkzderUSatXr1b+/PnNLs3+e588eVKxsbE6cuSISpUqpbZt22rmzJlKkSKF/a7yjiY5OVmvvfaatmzZoi1btmjixImaMGGCSpYsqa5duzpsII2XyysVSD16F7DUqVNr7969SpMmjTw9PdW4cWM1btzYYfpN58yZUylS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
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Clearly, only a few classes have any covenant diversity. Paladins and Monks only use one covenant, and for most specs, one covenant is a clear winner in popularity. In 9.0, the launch of Shadowlands, swapping covenants not only reset all progress in terms of power progression, but swapping back to a covenant one has left was time gated behind a two week waiting period. I would like to highlight the failure of the system in regards to allowing players to choose freely, indicating an imaginary balance between covenants for each class, but the mandated friction only compounds the issue of covenant imbalance.</p>
<p>To follow up on this, we should compare IO score by covenant for each class.</p>

</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[8]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s1">&#39;Spec&#39;</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Rank&#39;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">&#39;Covenant&#39;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">Dungeon92Ranks</span><span class="p">,</span> <span class="n">dodge</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">&#39;seaborn-white&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Player Rankings by Covenant per Spec&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Class&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Score&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">(</span><span class="n">rotation</span><span class="o">=</span><span class="mi">70</span><span class="p">)</span>
<span class="c1">#plt.gca().invert_yaxis()</span>
<span class="c1">#plt.ylim(3100, 3900)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">bbox_to_anchor</span><span class="o">=</span><span class="p">(</span><span class="mf">1.05</span><span class="p">,</span> <span class="mi">1</span><span class="p">),</span> <span class="n">loc</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span> <span class="n">borderaxespad</span><span class="o">=</span><span class="mf">0.</span><span class="p">)</span>
<span class="c1">#sns.set(rc = {&#39;figure.figsize&#39;:(18,8)})</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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JScny8nJScuWLftTuHV/a5qH0a9fP/n7++vo0aOqWLGiDhw4oG+//VZLly5V4cKFtWPHDr3//vsPtawmTZqoZcuWevfdd7Vy5co0ocuDZMuWTbGxsbafr1+/bvt/1qxZNWzYMA0bNkyHDh3SSy+9pLp166pEiRJplnH79m3b/62BS65cueTq6qoyZcpow4YN2rJly18Osl6uXDlFR0fryJEjqlSpku3xpKQkTZ48WQMGDFC+fPkUFRVl+11UVJTtToXNmjXTxx9/rNKlS6tmzZrKli2bPD09lTVr1r8cwH7Pnj1/+1486LOQXvfXffv2bVtY5OnpqSlTpqhMmTL/annBwcEqUqSIvLy85ODgoEqVKumNN95IU6u1++j96/T09FTJkiW1fPnyPy0zd+7caea5ceOG3N3duWsfAAAwDF32AABPnJs3b6p8+fJycnLSjh07dOHCBd25c0fSvbCmQYMG+vDDD22te5ydndWwYUMtWrRI0r2BsEeMGPFQ3bf+KGfOnOrdu7dtnKhbt24pb968KlCggO7evavly5crLi4uTUuov1O0aFE1aNBA9erV08cff/zQNVSpUkX79u3TrVu3lJiYqBUrVth+N2DAAIWGhkqSypQpo2zZstlaQt0vPj5e69evlyStXbtWlStXtnXta9Wqlb788kuVLVvWFiLdL1u2bOrfv7/efvttXbhwQdK993TkyJE6duyYPDw85Ofnpx9++EEWi0VxcXH66aef5OfnJ0mqUaOGbt68qeXLl9v+RoUKFZK3t7ctkLp165aGDRumuLi4B74XD/osPIizs7MtiPujc+fO6dixY5Luddf08fGR9P+DzEv3ult+/PHHOnr06D+u6+eff9YHH3xgCxGTk5O1atUq1axZ0/ac9evXKzExUXFxcdq6dat8fX1VtWpVRURE6ODBg5KkS5cu6c0331RqaqoaN26sVatWKTExUXfu3FGXLl3SjGcFAACQ0QikAABPnIEDB+rjjz9WixYttHfvXr366qv68ssvtX//fkn3uu2Fh4en6W724Ycfat++fQoICFDbtm1VpEgR2x3i/q0ePXrozJkz2rRpkxo0aCBPT0/5+fmpT58+6tWrl7Jnz/7Abnh/9Pbbb2vPnj1pBvt+kCpVqqht27Zq27atevTooWeeecb2u27duun1119X8+bN1bZtW3Xp0kXFihX7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/f1Onz6txYsXy9PTU4mJiSpVqpTy5s2rPHnyKE+ePIbXY30v9+zZowULFqh///4qVqyYQkNDFRERYVdjHVm32xkzZujo0aOqXLmyjh49qlu3bunSpUvauHGjPvzwQ3l5eZlc6T1OTk5KTU3VmjVrNGLECB05ckTXrl3T4MGDdfXqVY0ePdrsEtOw7kN//PFHzZ49W5cvX1aNGjX07LPPqn79+qpRo4bhNd1/x+GsWbNq7969ypYtmzw9PfX888/r+eeft8vxw6x1h4eHa8+ePfr555/l6+ursLAw5c6dWyVLltT69etVuXJl077zrTWePHlSt2/f1hdffKHmzZurXLly8vX1NfxCuHX7tlgsOnv2rAYMGKC8efNq7NixOnPmjHLlymV6GCX9/3nQO++8o1u3bqlcuXI6cOCA4uLidOvWLe3du1cjR45UtmzZTK4UT6onssvexYsXtX//fs2bN0+RkZGqU6eO2rRpo6efftrUuvbt26f+/furRYsWat++vQoXLixPT09J9+4Y4uLiouTkZL366qt6//33VahQIVPrtfrhhx80Z84ceXp6qlixYjpz5ozee+8908eW+KOEhAR9+umn2rVrl/r06aNz587pwIEDmjhxomkHg9ZQYu3atfrtt9/UsWNHjRkzRl27dtWkSZOUM2dOffvtt3JzczOlvn9j/PjxatSokS2skO69525ubtqxY4d++eUXjRs3zrT6ZsyYIT8/PxUrVkweHh4KDQ3VmjVrFBoaqvDwcJUvX17+/v4qXry4ihUrluH1WP/2o0ePVr169ZSSkqIrV66oU6dOGjFihGrXrm1698E/OnTokGbPni0PDw9dvnxZTk5OGjx4sGktkKzvYWhoqLJmzaqff/5ZwcHBKlCggE6ePKly5crpww8/NKW2f6N169aqUKGCunTpoqpVq+rSpUvKmTOnLdg3sym9dd1LlizR0aNHlZiYqISEBH3++ec6dOiQqlatakpdD7J//36NGjVKd+7csXV/rFWrlqmtoO9vUXDy5EmdOXNGhQoVssv3737Wv//Bgwe1d+9ebd26VdmyZbPtL8uVK2dabUlJSVqyZIlWr16t559/Xh07dlRUVJScnJzs4iTQYrHo7t27cnJy0q5du3T+/Hm5uLioXLlyunTpkooWLapt27Ypf/786tatm+ndcu9vTb5+/XoNGzZM7777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eUaFCxc25ftyw4YN+vjjj5WYmCg/Pz916NBB1atXl2R+z4BLly4pKipKxYsX17hx42zDGhQrVkzFixfXxx9/rG7duqlo0aKm1wpIT0AgJd3b4SYnJ8vFxSXNRnfo0CFVqVLFxMruDSLo6uqqhQsXasuWLcqTJ4+8vb1Vvnx5Pf3006aFJg9iPWk+ceKEPvzwQ3l5een111+3m5ZH998aNiUlRc2bN9fdu3d15swZHTlyRHfu3DHlbhx/9OGHH6pVq1a6efOmjh07poEDB+qdd97RK6+8YjfjYPyVpKQkrVq1ShMnTlRUVJSmTp2qevXq2X5/9+5du2l1aP0szJ8/XwULFlSdOnVksVh09uxZ3b59WzExMWrRooVhBzPWJv1z587V6dOn5eDgoBIlSqhChQoqWbKk8uXLZ/rBgfW9+PXXXxUSEqLevXtr1KhRGjJkiN5//33ly5dPX375pWkH2NWrV1e7du308ssvy9PTU5988omtW4Q9ffYeJCIiQp9++qleffVVDR8+XIsWLZIkffLJJxo8eLDpt4r+9NNP1bx5c1WqVEnXrl3Trl27dPjwYV2+fNnWHaVJkyam1mh15swZubi4aPv27apRo4Zu3bqlAwcO6Pr164qNjVXr1q1NuegUFBSkkSNHKioqSn5+furTp4+qVaumCxcu6O7duypWrJhdflY3bdqkvXv3KjQ0VO+8846eeuopXbt2TadOndKBAwfk4+NjeHfy/fv3a968ecqTJ49y5MihypUr21pubNiwQUlJSerVq5ddnPTv2bNHa9asUbVq1eTj46PcuXPr559/1tatW3X48GF17txZvXr1UrZs2Uzf10v//x0ZGBio+Ph428DH0r391O3bt+120GNr65SffvpJy5YtU86cOVWsWDG1bdvW8HE4z58/r+LFi2v+/Pl69tlndf36de3YsUMHDhzQxYsXNWDAAD333HOG1vSwEhMT1a9fP82dO9f2WGpqqvr3769+/fqpdu3apn1W7969q8OHDytr1qxasWKF3n33XdsFk19++UU7duzQrFmz0tx4ISNZ34fjx4/r0qVL8vf3V3BwsH755Rft2rVLFotFK1asML2V9ocffqgyZcrohRde0IIFC3To0CFJ98bgSkhI0J49e7Ru3TpTawTul+m77EmyXZGU7p1spaamysnJSVWqVDH9gMBa14YNG9S8eXO5uLjo3Llz2rFjh9auXatOnTqZ1hLhr3zzzTdKSEjQqVOnVL9+fXXs2FGjR49W9erV1bNnT7PLk/T/zc8XLlyoO3fuyMvLSzVq1FClSpVsB7FmsVgsti47YWFhyp07t7777jsNHjxYbm5ukqRz587ZdSDl4uKi559/Xnfv3tXq1av12Wef6aOPPlLTpk1VuXJl/fzzz5oyZYrZZdq284iICP3888965513dPv2bU2cOFG5cuVKMwCuUVfWihYtqvPnzysyMlKdOnXSsWPHdOrUKZ0+fVqurq564403TOsKZ2V9L06dOqXixYtr0aJFqlChgsqWLatevXqpZMmSpp34WSwWjR07Vr/++qteeOEFeXp6Kjw83HYSZY8n+PeLiYmRh4eH8ufPr3bt2unEiRMqWrSoFixYoOLFiys0NNT0MCoxMVFXr15Vr1695O7urvbt26tLly56/vnndebMGW3YsMFuuppZLBZFRUVp4cKFOnz4sIoXL64KFSqobt26unHjhn744QfTupL7+fkpKChIkydP1vbt29WvXz85ODioU6dOat26tTw8POymBen9GjZsqH379ik4OFjTp09X0aJF1aBBAzVo0EBHjx61tQAwUo0aNVSiRAmtWbNG169f14YNGxQUFKQiRYqoVKlSatiwoektjaxSU1OVLVs2HTt2TAcOHJCnp6dKliypDz74QHnz5k3T8tnsMEr6/+OlkJAQrVu3TitXrlTfvn3Vrl075c+f3/A7Kf6T+8dlW716taKiotS5c2ctXrxYSUlJprQsT0pK0qFDhzR48GDFxcWpXLly8vHxsR1v7t271y5vVGN9L11dXVWtWjV17txZL730kurXry83NzdFRkbKx8dHknmf1dTUVJ09e1afffaZnJ2dVblyZTVs2FABAQEKCAjQ2bNnDW1laj1nPHnypOLj4yXduzmNr6+vYmJidPz4cdPDKOleQDpkyBA5OjqqW7dueuutt1S5cmWlpKTIw8PDNuaWPbTSBKRM3EIqNjZWV65ckZOTkzZv3mxrEWOxWOTg4GAXB4Fbt27VsmXL1KZNGx0/ftw20FxsbKxOnTqlQ4cOqU2bNsqTJ4/Jld6TmJioSZMm6amnnlJqaqqOHTumkiVLysHBQXXq1FHx4sXNLjGNXbt26ccff9SBAweUJUsW+fv7q3379qbeteqnn35Srly55Ofnp9WrV2vnzp26cuWKpk2bphMnTuiTTz7Rd999Zzfdtv6K9Qs5NjbWFvht375d69at086dO9WmTRsNGTLE9C8668nezJkz5eTkpA4dOmjGjBmKj49XhQoVFBISYnizfkkKDg7WN998Iz8/P3Xu3FnR0dEKDg5WXFycXV1BjY2N1eHDhxUeHq7z58+rT58+euWVV/TKK6+oYcOGZpeniIgIbdq0SWvWrFFYWJiKFSumfv366emnnza7tL8UGxur//3vf3r22WdVqlQplSlTRjlz5tTOnTs1ceJEJSYmqlevXmrbtq3p247Vzp079f333ysoKEglSpRQly5d1L59e1t4bg/u3LmjmTNnatu2bapataoSEhJUtmxZubq66vTp03r33XcNr8m677FeOR81apQkaceOHRo3bpxOnz6t7du328U4I3/F2lUra9as2rVrl65cuaKwsDB5eHho/vz5htYSHx+vAwcOKC4uTkePHtXgwYN1/vx57d+/X2fPntXNmzf18ssv28VFHOvxZUpKipYuXaosWbLo1KlTio6OlrOzs/LmzasXXnjB7kIeK4vFouXLl2vWrFk6f/686tWrp2+//dYujpf/qF27dmrevLlSU1O1fv16xcbGqnTp0hoyZIhpn4UJEybot99+U65cuRQbG6v69evL09NTu3bt0vjx402p6UGWLVsmLy8vlStXTlmzZtUPP/yg06dPa//+/fLy8lLt2rXVv39/uwjOP/vsM2XJkkUhISEKDQ1VlSpVFBcXp9KlS+utt94ytBaLxaIWLVrI29tbgwYNUvXq1e1qiI2goCBt3rxZo0aNUmpqqm7cuKE33nhDc+bMkWR+d0Lgr2TaQOrWrVv69ttvtWDBAhUsWFATJ05UuXLlzC4rjTNnzujbb7/VqVOndOnSJTVt2lSvvPKK3XR9s7J+GUVHRysiIkJ58+b903gC9rKDs9Zxfz1RUVHau3evli5dKnd3d02aNMm0+nr16qW3335b5cqVU0xMjF577TVdunRJpUqVkrOzs8qWLatXXnnFtPr+ifV9tY7F9txzz6lGjRq6dOmSEhISVLp0aVs3VHv5TFgHv4yPj1eVKlU0YMAALV68WDdu3NCgQYNMOfnfu3evAgMDVaxYMQ0dOtRuTvCt23pUVJRu375tu9I3ZMgQJScnq3DhwnY5VtOZM2e0ZMkSlS5d2tC77fwb586dU9++fVW8eHHVrVtXzs7Oyp07t8qWLassWbLI29tbzs7Oph/4WywWWw0Wi0XOzvcaUq9du1affvqpGjZsaDd317M6evSoKlSooOvXr2vbtm06evSozp07pwYNGpjaPXvy5MkKDw/XuHHjbPvFPXv2KDw8XO3atTOtrn/yxxuVnD59WhERESpQoIDhF54SExN1+PBhjR07VvHx8erfv7/KlCmjChUq6MaNG1q7dq26detmaE1/5+bNmwoKCtLOnTuVL18+vf3220pMTNS5c+e0b98+3bx5U//73//s4ntR+v/v8w0bNujs2bMKDQ3V2LFj5erqqsuXL2vnzp12uT+Ni4vT5MmTNXz4cNtjBw8e1A8//KCePXua1sUwISFBBw8eVMGCBXXo0CEdOHBAO3bsUNu2bdW/f39Tavo7N27c0OjRo+Xm5qbcuXOrdOnS8vT0lLOzs7y9veXi4qICBQrI2dnZtGM563oTEhJ0+fJl3bx5U76+vjp9+rSCgoIUHBys119/3ZS/9+7duxUUFKT169erWLFiCggIUJ06dezi/K1Xr16qVauW7VxixYoVOnnypN566y3b9xBgbzJtIGU1dOhQ5cqVS/v371diYqICAgJ06tQpNWjQQF26dDG7PEn3+kjv2rVLq1at0m+//WYbo6Nv3752cYJiNXjwYIWHh+vcuXOqXbu2OnfurN27d6t+/fqGjynxICkpKRo7dqxOnTqlSpUqqW7dunr66ae1Z88eVahQQblz5zalrhMnTujLL7/U9OnTbY/16dNH7733nq5du6bSpUsrb968dnOw+les4c3EiROVNWtWdejQQStXrtSWLVtUrVo19evXzy6aK98vJiZGM2bMUL58+dSlSxedOHFCH3/8sUaPHq3SpUsbcrBlXcf9YxxFRkbqm2++UVJSkjp06GBXgfno0aN18eJF/e9//1PlypV15coVxcbGqlixYhzM/AdHjx7V6NGj5ezsrNq1ays5OVnJycny8PDQ008/beseYRbr5zQ8PFwff/yxLBaLChUqJF9fX/n5+Sk0NFRly5a1qxacZ8+etW0/rVq1Ups2bWz7ILOv7F+7dk1jx45VyZIl1bJlS+XMmVMffvihWrZsaTd3hLOyvlfWmwQcP35cLi4uql+/vlq1aqWtW7eqX79+pryfCQkJWrRoka5du6bk5GRFRUWpYMGCOnLkiGrVqmU3J/tJSUk6fvy4Bg8erEKFCqW5Tf2xY8d09+5dBQQE2M3FGuneBbvBgwerY8eOCgwM1KxZs3TkyBH5+vraXRdo6/HHjh079Msvv8jJyUnPPfecypYta9rA29bt5ujRo5ozZ46qVKmibt26KSkpSQcPHlT16tWVmppqC/btSXJysg4ePKjffvtNx48fl5ubmwoWLKjixYurYsWKpvd6sP69Z8yYoZMnT9rGAzx//rxu376tqlWrGlrPsWPHlJKSoty5cys6Olqurq5KTk7W5MmTtX79enXv3t2UFrn3s1gs+vjjj7Vt2za5u7urVatW2rFjh0aPHm03Xe2Bv2J/e8hHwPpln5iYqBEjRsjT01MJCQk6cOCA1q5dq6ioKNMHZL2/JUJ0dLQKFiyod955R8nJydq1a5dWrlyprl27mn53i+TkZDk7Oys4OFhZsmTR8uXL1blzZ5UtW1ZvvPGGqlevrpdeesnUGq2s7+nq1auVkpKiVq1a6auvvtKuXbsk3XstP/zwg2n1/frrr7Y7g0n37g6WO3dulSxZ0u7utPR3rC2J9uzZo0WLFumbb77RnTt39Nprr2nRokUKCgpSy5YtTa7y/z8Lly5dUmhoqPz9/VWxYkU5OTnp1KlTCggIUOnSpSUZOzbC+vXrtXr1amXNmlU+Pj66efOmVq5cKRcXF9MDKet+MzQ0VEePHtWiRYtsY+5NnjxZlStXttvBbR8HFotFFStW1NSpU7Vo0SLlzJlTzz33nK5cuaLNmzfbxo4y82TVOr7dkiVLVKdOHUVERGjr1q06der/2rvPsCqv7O/jX4pIUwQivSggELABYkHB2FCxl4jGHjsax5jYorHEhBhNsUVjiWjsvWFDREEBEaSoIIgogihFaYL0w/PC55zRmUxmMv8J90H3500S4Lr45XDKvte991r32LRpEzo6OooG7MrCxsaG4OBgwsLCOHPmDNu2bcPW1pZJkyZJfnzT2NiY2bNns3PnTubOnUuzZs1o1KiR5OuPP3Lu3DnFzaaioiJSUlLYv38/Pj4+dV6Mkr8WioqKaNiwIZ9//jkymYz4+HiioqJo1qwZPXv2rNNMf6RBgwa0bt2aVatW0bhxYyIjI0lMTCQuLo7Lly8rRW9FOfln5KlTp+jevTtt2rTB0tISfX19MjMzuXr1Kl988YXUMd8gX3988803tGnTBhUVFQIDAwkNDaVp06b07dsXIyOjOs0kv6d/7NgxHB0d6du3L/Cqh8/Vq1dp3bq1Uh3nkpPJZKirq+Pm5kbz5s0ZNWoUt2/fJiYmhmPHjqGioiJ5QUr+946IiODLL79UrD+ePXvGhQsXsLOzq7Oei4mJiQwbNozGjRujq6uLo6MjqampFBUVMXToUJycnJSilYGamhpffvklpaWlhIeHc+bMGZKTk1m8eDE+Pj4MGjRI8j6lgvB73uqC1Lp169DS0mLUqFFUV1cDMHv2bKXq27BmzRpu3bqFtbU11tbWtGjRAjs7O9avX68UO03kd3VCQ0Np0aIFBw4cwNPTk5kzZ2JjY4OOjg6GhoYSp3xFfhEXHh7O+PHjSUhIYMGCBfTu3Rt/f38GDBgg6Z39gIAAhg4dSvv27TEyMiIqKkqxeJGP2q4PysvLsbW1ZeTIkQBs2rQJAwMD1q5dK/kFoJz8wmnWrFk4OzuTk5NDRUUFrVu3xtvbm7Zt29ZpHvlFVWxsLKNHjyYlJYWXL1/y4Ycf4ubmVud5/lVGeDVauXnz5sDfH8cRI0bw22+/Kf7mwp8nX1wbGBgwduxYVqxYwaVLl/jyyy/f2OEh5c4JecY7d+6wZcsWVq5cyVdffYWJiQkBAQFKczTqdeXl5RgYGDB48GAGDx7MuXPnOHToEC9evJAkz+v9o6KiojAyMuLTTz/F0NCQW7duYWNjo5Tv9aqqqpSUlJCeno61tTUbNmxg/fr1vHz5khs3bkhysSV/LWRkZBAQEMD27dtp164do0aNYubMmXWe54/Id3M8ffqUR48e0bhxYwYOHIi6ujoPHjxgxIgRiklgyrA7Sv7erqenR3FxMbt372bAgAHAq/WIsu2Okq/rnz59ire3N3PmzCE7O5ukpCSSk5NJTk5m8ODBdZ5LTU2N2tpaUlNT8fPzw9DQEJlMhq2tLYmJiURFReHp6Vnnuf5IbW0tqqqqPHz4kF27dnHlyhW0tLTo378/48aNY/jw4YqihdS7+XJyctDU1HzjZIOLiwvfffcdL1++rJOCVG1tLebm5vTr14/33nuPMWPGYGlpSXx8PKtXr2b27NlKV+TR0dHB29sbb29vcnNzCQkJ4dChQ8TExPDDDz9IHU8Q/olynAX7H1NVVaWmpoZbt24xaNAgnj9/zueff8758+c5f/681PGAVxkrKip49uwZu3fvZuzYsWhqahIZGcnPP//M06dPpY5ITk4O/v7+ZGdnM2XKFFxdXXn27Bk5OTkUFRURFRWlVHd+5B+azZo1Iy4ujrCwMExMTNDU1ERbW5tGjRpJlk0+Hez58+f4+vri6+tLYGAg7dq1A1DKC5R/RVNTk0WLFjF+/HjWr19PRUUF3333HQYGBhgYGKAsp4CTkpKwtbXF39+fr776ismTJ1NbW8uqVavq9GJVJpMBEB0djaamJp6enkyePJnJkyfj7u6Or68vDg4OdZbn3/Hy8iI3N5fp06dz+PBhUlNTOXfuXL3ZxaeMgoODuXjxIjExMWzfvp3z58/z4YcfUlBQwIIFC3j48KHUERUqKyvp3Lkz+/fvJzc3F2NjY8U0Q2W5SJW/x8TGxrJ582ZiYmLIyckBoHv37jg5OdG9e3dJsqmqqpKfn8/XX3+Nvr4+mzdvZtasWSxYsIA1a9aQmZkpSa7/RIMGDZgwYQLx8fHo6enx8uVLVFVVOXnypGRH3eHVFKsLFy6wceNGmjZtyty5c+nQoYNi97MykBdz582bR1JSEtu3b2fEiBGKozJ1NZb+z+rYsSMRERGcO3eO27dvc/bsWS5cuIC3t7fU0X7X/v37iY2N5erVq5iYmNC9e3f8/Pz45JNP0NPTkySTiooKPj4+zJw5k+DgYEVx98WLF7Rv316STH9EviY5ceIEpqamXLlyhW+++YakpCTmzJmDkZGRYr0sZTFKJpNhbGyMp6cnEyZM4Ndff+Xhw4fs27cPU1PTOhsOoKKiQpMmTfDz8yMlJYVZs2aRmprKoUOH8PHxQVtbm6qqqjrJ8t8wMjJi5MiRHDt2jBUrVgCvrkkEQZm8dT2k5NV8+bG3FStWsGjRIrp164aTkxOLFy9m165dStEHRb4IeH3SV35+Pjdv3qRXr14SJnslIyODv/3tb6SlpWFtbc2wYcPo06cPe/bsQSaTceXKFY4dO6YU/UTi4uJo0KABdnZ2NGzYkPz8fG7cuMG+ffuwt7dXPNbKoL5NB3udvNCbnJzM+++/T7NmzWjYsCGnTp3Czc0NOzs7yfu2yO9Unz59mqKiIkaPHq1odF9aWsqLFy8wNTWt8zt/X3/9NS9evGD06NFYW1tLtnj+PfLH4u7duzx58gRPT0+OHDlCSkoKUVFR+Pj4MGHCBMmPENdH8fHxip1l/fv3x8vLi8jISNTV1TEzMyMqKop58+bh7Ows6d1o+esmMjJScczk8OHD7NmzBysrK1RUVN7of6cMoqOj2b9/P3l5eRgZGeHq6kpiYiJFRUWSHI+Sv/ft2bOHly9f0rlzZ7Zs2cLEiRNZt24djo6OLFy4sM5z/Te2bNnChQsXMDExwczMjCVLltTp75c/lvJprvr6+op1W3h4OOHh4UyZMkXSQplcQUEBqqqqPHv2jA0bNrB27Vrg1U29TZs2oa+vzyeffKIUkzPhn3e9ZGZmEhUVRWZmJsnJyYwaNYoPPvhAuoB/QL52unnzJs2bN6d379507doVY2PjOs+yY8cOPvroI/Lz8zEzM+PQoUMcPXqUBw8e4OHhofRDaj766COWLl36RruAzz//nAEDBtC1a1cJk71SW1tLeHg4Xbp04caNG2zfvp0nT57Qs2dPPD09Jeu5uHXrVpKTk7lz5w5BQUGSZBCEt81bV5CSe/jwIX5+fqirq9OvXz+mT59OaGgoly5d4quvvpI0W2RkJO7u7pw/f57Vq1djZmZG//796dWrlyQfqv9OVVUVwcHBzJ8/H5lMhoaGBr169WLBggVKc1xv7ty55OTk4OjoiLu7Oy1btkRNTY2LFy8CKBqLKpv6MB0M/n5xcPr0aU6cOMF7773Ho0ePsLKywsLCgvz8fJYtW6YURxHg1cX1qFGjyMrKonPnzgwdOhQXFxfJdqLV1NSwc+dOIiMjqampoXXr1nTo0AFra2vMzc0lyfQ6+d/3xIkTlJWVMWrUKEpKSpDJZDRu3FjRS074c+QXfkFBQURERBAWFkarVq3w8/NTql1xr5sxYwaVlZVMmjSJ1q1bExYWRmFhIS1btqR169ZSx/snJSUlNGzYkLCwMC5cuICVlRXe3t7Y29tLlunnn3/G3t6eqKgo7O3tGTFiBHv37sXNzU3yXnH/SP4cLSws5MKFCyQnJ+Pt7U2nTp24fv06KioqODk5SbbDeNeuXWRnZ+Pq6oqlpSWOjo6EhYUpCrnKYPXq1Tx9+hQbGxuKiooYNWoUpqamaGtrk5SUxMqVK9m/f7/UMf/JZ599Rk1NDU5OTlhaWuLg4IC1tbXSFM7kXi+gVVZWUlxcjK6uLocPH+b8+fPk5ORw9uzZOr3RXFZWRkxMDB4eHsyePRtTU1M8PDxo3bo1qqqqNGjQQNJd+f+Jbdu2UV5ezrRp09DQ0KC0tBQ/Pz9++uknDAwMpI7H/fv3mT9/Pk2aNKFr166KI3NSka+T5FPcjx07xvz58xkwYIBSbHIQhPrsrS1IAZSWlpKfn4+lpSUnT57k+PHjTJkyhc6dO0uWKSsri+HDh2NoaIijoyMdOnSgvLycR48ece/ePbS1tfH391eKD4OKigpUVFQUb7TTp0/ns88+4/r166xevZotW7bg4eEhccq/u3PnDsHBwSQkJKCiooKbmxuurq5YWFgoxSjW+kz+QTxz5kzmzp3L8ePHUVNTo7KykqSkJDp37szUqVMl3x0Fby5eHz16xIEDBwgLC0NVVZXevXsza9asOssifzyuXr1K06ZNcXR0JCkpiXPnzhEREUGrVq1Yvnx5neX5IzU1Nfj4+GBiYoKfnx8dOnSQOtJbp6SkhCNHjhAYGEhFRQX29vbMmzcPY2NjpSnmwquBC/Hx8XTs2FHpdm6+vgPy0qVLxMbG0rhxYyZMmMCQIUNQVVWV/LHMy8vj7t275OTkkJKSgp+fH5MnT2blypU4OztLmu0fyd+jvvvuOzIyMrC2tubq1avAq+OPw4YNq/PpTLW1tWRkZHDr1i12797NgwcPaN68Oba2thgYGHD9+nVGjhzJiBEj6jTXv5KZmalYe6SlpWFvb4+3tze1tbXcu3cPGxsb+vfvr3juSkn++RgfH88PP/yAr68vsbGxFBYWoquri6WlJePHj1eqC2z5c/Snn36iurqaEydOsG7dOkXLg9zc3DpvZv7w4UP09fXR1tbmypUrZGRkkJaWRllZGVZWVrRv316ppk//nidPnrBixQpiYmJwd3fHyMgImUzG119/LXnvKHhVfHzy5AmpqalERkZy+/ZttLW1GTdunFIMhoiMjGTDhg188cUXtGzZUuo4glCvvVUFKfmHfVJSEhEREYSGhuLm5sbw4cNp0KAB6enpSnORFRMTw9GjR4mOjkZLS4u+ffvi5uZGcnIy48ePlzrePwkJCeHMmTNK2Qzv9xZ5cXFxBAUFER0djZubG4sWLZIo3dvjxYsXfPnllyxcuJBPP/1UcfR106ZNjBs3Dl1dXckXMfLff/PmTXJyctDT06Nt27bo6Ohw9uxZcnJymDhxYp0XzjZu3Mi1a9fQ0dGhW7du+Pj40KhRI7Kzs5WqWHr9+nVCQ0O5ePEi1tbW9OnTh44dOypVxvpIPlTj9V1mGRkZ7N69m3Hjxkn++L4+odTR0RFNTU2OHj3KmTNncHBwYObMmZLuOPo9U6dOxdfXlw8++ICLFy+yZ88e2rZty9y5cyUpisvfe6qrqyksLOS9996jqqqKKVOmkJGRQffu3ev82NufsWTJEvz8/DAzM6OyspIbN26wZ88eunTpUufN7E+cOEFISAhVVVX07t2b0NBQIiIiaNGiBZ06dcLFxYUOHTpIXtyBv68/5BNJ8/PzCQwM5Nq1a+Tk5GBlZcWPP/6oFK0N4M1dm+Xl5QwcOBB4tVs7NDSUqqoqpk2bJnHKf1ZUVMScOXP45ptvWLhwIWvXruXWrVvU1NRIUpwYNmwYJSUl9OvXjx49emBqakpBQQFpaWlER0fj7OwsSZP1/4RMJiM5OZknT57g4eFBZWUlYWFhtGjRAmtra7S1tZXi5qJcbW0tL1684OLFi9y4cYMJEybw/vvvSx2L2tpaUlJSMDMzE+0MBOH/6K0qSMlNmzaNLl26YGxszMmTJ7l79y7Lly9XipGclZWVb9x5kslknD9/np07dzJx4kTF1DWpjRw5ko4dOzJs2DAsLS1ZtWoV7dq1o2fPnpSWltbZqNU/Y+PGjRQWFgLg4eFB9+7diY6OBsDd3V3CZPVbSUmJYuJjVFQUL168ICwsjA8++ID333+fmTNncuzYMYlT/n2hnZuby4wZM3B2diY+Pp6WLVtiZ2dHYmIi8+bNw8TEpM6zlZaWkpeXR1JSEmFhYSQlJWFpacmPP/4oeUP7pKQkZDIZ+vr6FBcXo6GhQXV1NRs3buTixYuMHTuWxYsXS5qxPvvHgnlNTY1S7OL5R2VlZYwdO5aKigr69++PtbU1UVFRnD59mu3btyvFJMj4+HhCQ0Pp1q0bISEhTJ48WfHeVFlZyYgRI9i4cSMWFhaSZfzyyy95/vw5paWldO/enaFDh9KoUSPJi/V/5OHDhwQEBODm5ka3bt1o1KiRIqsUuceMGcOiRYve2E0mz+jr66t0u8zg1bTZs2fP4u3tTd++fWnRogXJycmKcfHKdoG/efNmDh06hK+vL5MnT1aqATWvkz//jh8/TnZ2NkOHDuXbb79l7dq1xMTEsGHDBnbt2lWnme7du0dJSQnV1dX8+uuvPHjwAGNjY7y9venatSs6Ojo0atRI8s/2fyT/LDp27BiHDh3CzMyMJ0+e0Lx5c3r06EH79u0lL6zI/94nT54kIiICX19fWrZsiYaGBs+fP2ft2rVv9N0VBOHt8NY1BXnw4AEvX75k7NixAHh7exMVFcXJkydxc3OTvJAiL0ZVVlaioqJCgwYN8PHxwdDQkFOnTvHBBx9IPsmopqaG0aNHExISwrhx4xQTlqZPnw4g+WP4utdHbMfHx9OzZ0/27NlDcXExO3fuJCMjg+PHj0sds15bunQprVu3xtHRkZYtW6Krq4uqqipz587F1NQUX19f4Pd3qtUl+ULmxIkTDB06FAcHB54+fYq9vT0nTpygS5cudVqMkvddqqysREdHBx0dHSwsLHBzc2Pfvn0YGRlJvmCVXyw1btwYXV1dHB0dSU1NpaioiKFDh+Lk5KQUhfz6qLa2lqqqKjQ0NIiMjKRTp05UV1crilHyf1eWi1Q1NTWmTp3K6dOniYuLw97enmXLluHr66s0fY80NTW5ceMGgYGB1NTUUFJSwtSpU9HV1eXRo0eYm5tLWoy6efMmd+/e5dtvvyU1NVXReLtx48asW7dO8s/2f1RWVoaWlhbZ2dncv3+fe/fukZqaSrt27bCxscHY2LjO36Pu3LmDiorKG0Wn2tpamjVrhrOzM0FBQTg5OSldcW/IkCG0bNmSyMhIvvrqK3R0dGjfvr1id5kyvM5f3wl5/fp1pkyZwsGDB9mwYQOtW7dmwoQJ9OnTR+qYb5D/nd3c3Fi3bh1z585l9OjRANy6dUuSQvnBgwfR09NT7B5t3bo1Z8+e5dSpU2zevJnevXsrzVH818nXZ7du3WLKlCl4enqSkpLCzZs3+e2330hOTq7Tlga/R/73trGxITQ0lEWLFqGvr4+XlxdpaWlKdf0hCML/zltXkKqsrMTc3JyKigrFQqpx48bk5uZK/ka2a9cuWrVqhaur6xuFKQ0NDfT09CgqKlKKBauamhoDBgxgwIABb0yEGz58uNJNhHu9GfO4ceMoLi7Gy8uLfv36ceDAAWbNmqUUU3jqq/T0dMLDw8nJyaGoqIgbN25gYGBA165diYyMpLKyEm1tbUD6Bbf89xcUFNCmTRvOnj3L2LFj8fLyorKyUvGcras7/urq6oriuLu7OwMGDKBFixYYGxsrxTjo2tpazM3NFY1Cx4wZg6WlJfHx8axevZrZs2cr/rbCn1dQUMDWrVsV/csCAwPfOLKnbE3iVVRU+OCDD+jWrRtJSUncu3ePrKwsHB0dJS82w6sCb2VlJXv37qW8vJzQ0FAOHjzIRx99hLGxMYaGhkyYMEGSbD///DNubm4UFBTw8ccfK46+dOnShczMTJ4+faoUn+2vKyoqYtOmTSxatAg9PT327dvHgwcPCAwMZNeuXZSVlbF8+fI6L0bevXtX8TsrKytp0KABMpkMNTU1unfvjp+fH59++mmdZvpXXt/1ZGpqiqmpKe3atSM9PZ1du3Zx69Ytpdp5JP/cu3//PjNmzKBTp06MHj2avLw8tmzZwtWrV5WuICVnZWVFnz592LZtG1u3buXQoUNoaGjU+XNBJpPRvn17Dhw4wObNm5kwYQJaWlr4+Pjg4+NDfn4+WVlZdZrpPyFf9xQXF2NmZoaxsTEaGhq0atUKBwcH+vTpo7hGkmo3nzzjo0ePCA8P58cffwTg7NmzXLhwAWdnZwYNGlTnuQRB+Ou9lUf2Fi1aREhICN26daNnz55cunQJOzs7Jk2aJFmmmpoali9fTlRUFA0bNsTb25shQ4Yo7uZ+/fXXimk8yrD4/z3KPBHut99+w9zcnMDAQCZOnEjr1q1ZuXIlAwcOpE2bNlLHq9cePXrE2rVrUVVVpXPnzhQVFZGTk4OKigodO3ZUivHAr0tMTCQ5OZm8vDzy8vL429/+xuzZs/nyyy+xtbWtkwzx8fFERETQrFkzDA0NOXLkCDdv3qRNmzbY2tpy4sQJAgMDlaKvSFpaGitXrqSgoIDvv/+egIAAnJycGDNmDFVVVUp1QVUfTZo0iSdPnlBZWUmbNm2YPHkyz58/JyMjQ3GnXyrFxcWK/hzffvstdnZ2PHr0iKKiIqqrq4mJiSEoKEjyHlfw6nmampqKi4sLGzduZPDgwbi6upKXl8f58+c5fPgwO3bsoGnTpnWaq7a2lq+//porV66gqqqKubk5M2fOxMXFRVF0VMbjei9fvqS4uJjq6mr8/PwwNDTEw8ODvn37Ym5urni/quvX//Pnz1m8eDFz5879p75lAQEB5Ofn89lnn9Vppn9n69at2NnZ0bFjR0URXz74Y+DAgUr19y8vL2fx4sWkpaUxcuRIPD09lWLS6++Rr4VTU1O5fPkybdq0oUWLFjx+/JicnBzatm1b56/38+fPU11dTZs2bdixYwdlZWVkZGRgbm6Ou7s77u7uNG/evE4z/RlBQUF89tln2NraMnLkSD744ANJ2hj8HnkhLDg4mHPnzrFixQrFkezXvy8IwtvnrShIyd+kEhISSElJYcSIEdy9e5cjR46QmJjI+PHj8fLyknyHFLzqJRMeHk5gYCAJCQk0atQIFxcXXr58ybJlyyQ/v12fZGRkcOfOHczMzHBycuLu3bs8ePCAo0ePMnjwYPbs2cOBAweU4qK/vpIXJJKTk9m5cyf6+vr4+vpSXV1NdHQ077//Pm3btpV8wf3675f/+7Nnz1iwYAFPnz6lRYsWrFu3rs7yyIuivr6+mJmZERERwf79+wkNDWXw4MGKi2llsnXrVpKTk7lz5w5BQUFSx3lr3L17FwsLC7KysggMDCQkJISMjAz8/f0ZOHCgpIvsXbt28ejRI9q0aUNOTg4ODg5YWlry4MEDsrKy0NbW5sMPP5Qk2z+S73q+ffs2Fy9eJDs7m4qKClq1aoWnpycODg6S5EpMTOTBgwdoampiamrKnj17uHHjBm3atKFDhw507txZKQp6fyQtLY2HDx8SERFBeno6lZWVfPLJJ5IMgZHJZKxZs4aEhAS8vb1p3bo1LVu2JCEhgbVr17JkyRKlaGhcUlLC/fv3yczMJCEhgcjISLS1tenbty+tW7dm+fLlfPnll3To0EHyz8fXlZaWEhkZyf3798nOzqaoqAhDQ0M6d+5Mt27dpI73u0aOHMmwYcPw8vLC2NiYLVu20LlzZ0kmm/3www8UFRWhqqpKp06d6N27N0+fPuXy5cucP38eOzs7li5dWue5/hPy52FFRQXh4eHs379fUUxbuHCh0gyu+Prrr7lz5w6tWrWiXbt2WFtbY25uTqNGjaSOJgjCX+StKEjJHThwgLS0tHrTgPfFixdERkYik8no3bu30ixY6ouZM2cik8mIi4vjq6++AlAsClq2bMmgQYOUbidXfffdd99RXl7Oxx9/jKWlpVIttOFVQ2FVVVUMDAxwdnbG0tKSpk2boqWlhZaWVp1c/CcnJ7N27Vp++eUXqquruXDhAitWrGDevHlkZGTg7u6uVH2Z5I9Jfn4+27Zt49ixY8yfP58BAwYo1ejv+kR+Zz8iIoKsrCzatWtH8+bNyc/PB17tTpGy15FcREQEUVFRpKenU1JSgqurK87Ozri7u6Otra1Ur214dUH1yy+/MGzYMHJzc3n48CGpqancvn0bPz8/SYZXjB8/HmdnZ8aMGfNG8fnq1as0adKErl27smLFijrP9Ufk79slJSUEBgbSsmVLWrZsSXZ2Nk+fPuXu3bu4urpK2jvs/PnzxMfHk52dzd27d3FwcKB///54e3tLlul1P/74IykpKYwdO5YuXbqQm5vLqlWrOH/+PK6urnTs2FHyfjy/p6CggPz8fAoKClBXVyc3N5eYmBjef/99hgwZInU8Bflz9NatW/z8889s2bJF8b3Q0FCio6P59NNP6/w0QWZmJgEBARw5coTevXvTtm1bnJyceP/999HU1KS4uFjpbizLH8uCggLi4+MJDw/H3t4eHx8fKisr2b59Ox999BEWFhaSrelKSkooLS1VFHoNDAwICQkhOzsbXV1drKysGD9+vFiTCMJbSrmaWPwXampqkMlkqKurExMTw5MnT/jll19o06YNFhYWmJubK+0Wz0aNGinN4qq+SU5OpqysjB07dpCSksKCBQvo1KkTHTp0oFGjRgwcOFCSu2dvk9DQUAwMDCgvLyc+Ph5HR0dat26Nv78/t27d4quvvlKKaUfyBVRUVBR3795l9OjRpKenExoaSoMGDWjatClTpkwB6qbPVWBgoKI/1LVr1wgJCeGzzz7jww8/VPS9UaaClPwxMTAwYMGCBXh5ebFhwwYcHBzEa+i/JH9MDxw4QJcuXdDX12f9+vU8fvwYd3d3PvzwQ6U4fuDh4YGxsTHbt2/H1taWp0+fEhMTw/bt2+nWrRtjx45VigsAeYHv2rVr5ObmYmRkhJGRES1btuTp06d4enpKsuMwOTkZLS0t5s+fT3V1NWfOnFEUn5s1a0aPHj2U8si4vCfTmTNniImJoWvXrty4cYOTJ09iaWnJlClTJG8b0KdPHzw9PSkoKKBBgwY0aNAAAwMDSTO97ubNm2zcuBF9fX0yMzOZNWsWbdq0wdvbm549e9K/f39AOY5ryjNkZmayfv167t+/j7m5ORs3buTFixd06dJF8r/3P5I/ZtXV1TRs2FCxI1tXV5cmTZqQnJwsSWZLS0umTZtG8+bNadq0KWFhYdy5cwdTU1PMzMyU8iao/PW+d+9e0tPTcXFxITo6mgMHDjBz5kzmz5+v+FmpnqvFxcVERERw4MABunfvTs+ePXF3d6ewsJCTJ09SXl6uFJ9FgiD8Nep9QSowMFBxF3Ly5MncuXOH2NhY7t+/z3vvvYednR3Dhg2TfEEg/G8FBQUxcOBA4NXYenNzcxYsWAC8Wnxt3bqV9evXSxmxXpNPVWzcuDFjx45FV1eXXbt20aJFC4YNG8b169epqKgAlGPBDa92nUyfPp2ePXvy8uVL0tLSiI2NpUGDBqirq9dZztatW3P16lXu37/PmjVr8PHxoVevXsCrflzKsi3+X+nYsSP6+vqYmZlJHaXeUlFRIScnh9zcXEaMGMHmzZt5/vw5/fr1Y//+/bRv3x5ra2tJM8qLPHv27KFbt26KmyP3799n1apVvHjxQmkuAOQXnmlpaezfv5/nz58zbtw42rVrp2gmLYV/V3zesmULmzdvliTbH5E/noGBgaxbt47ExEQuXrxI8+bNyc7OJiQkRPGeJSX5dFJlExQUhImJCfr6+uTk5PDrr7/i7OzMvHnzSEpK4siRI3zwwQfo6uoqxWej/LPvyJEjdO/enf79+xMSEkJVVRX+/v6MHTsWJycnqWP+LldXV+7cuUNAQIDiBsnNmzcZNmxYnWdJTEykurpacW1hZGSEjY0Nx48fJywsTCmLUfD31/u1a9fYtGkTBgYG+Pr6Eh4ezpkzZ3B2dpa8j9R7772HgYEBBQUF3Lp1i++++w5ra2s8PDyoqKjA09NT0nyCIPy16n1B6vjx4yxcuBAAR0dHdHV16du3LykpKVy5coWXL18qxYJA+N8KCAhgyJAh9O/fn5s3bzJz5kzF90pKSmjWrJl04eq52tpa9PT0mDNnDuHh4Zw8eZJRo0axbt263704kPr1paKiQlVVFZGRkYrJf7169aJVq1a0atWKqqqqOs3Tvn17jh07xscff0zPnj2ZMWOGYifM5cuXFe9XykpFRUXSozpvi4qKCjQ1NVm+fDmZmZls376dsrIy9uzZI3kxCv5+kaKurk5gYCAmJiY4ODhgZ2dHq1atlGZ33OtDPry8vGjVqhUnT55k8eLFaGho4OLiwqJFiySZYvfvis/K/DoqKyvD2NiYEydOcPr0aZYtW0bbtm355JNPlL7nldQqKysVjat37tzJs2fPmDFjBo0aNUJLS4vS0tI3mjFLTf4Z/fDhQ3x8fNi7dy99+vShQYMGaGpqcu/ePaUqSMl3j5aUlJCXl8e4cePo0KEDISEhAIpjknUpMTGRYcOG0bhxY3R1dXn//fdJTU0lPz+fAQMGUF5ejpWVVZ1m+jPkO0vl75Pq6up4eXmxZcsWpZgAqqGhgaenJz///DM6OjpcuHCBhIQErl+/TlpaGuPGjZM6oiAIf6F63UPq9V4tcoMHD2bXrl3o6ekBKO3EOuG/V1NTw4ULFwgKCiIuLo6cnBxWrFjBwIED0dLSYs6cOfj5+Sn9TpT64tatW+zfv5/o6GgsLS3x8vJi9OjRqKmpSf7aki9cjx8/zpkzZ2jRogVhYWHU1tbSqVMnBg0aROvWrSXJVlNTQ01NDRoaGly9epW9e/fSqFEj1qxZI0keoe5duXKFO3fuMHz4cKqqqtixYweNGzfm008/lfzInvz3FxcX88svv1BZWYm6ujqVlZXEx8ezb98+pRgIkZ6ezs6dO7l37x4WFhasXr0aeJU/ODiYmzdvsmjRIkmyFRYWsnDhQpKSkujZsydLlixR/E0nTpzIwoULJWu2/p+IjIxk3759DBo0CC8vL0JCQtizZw979uyROppSy83NZezYsTx79gwLCwuWL1+Oi4sLAP7+/tjb2zN8+HClW3+ePn2a69evc//+fdavX4+amhqzZs1i7dq1ku+QeZ38venbb78lIiKCR48eMXToUMaMGYOdnR1Qtzuza2trKSoqYuXKlbz33nuMGTMGS0tL4uPjWbNmDdu3b1eKos4fkclkrFu3jqNHj9K/f3+6du2qaMa+YcMGSXe6y//ehw8fJj8/n2nTpim+l5WVhaqqqmS7YAVBqBv1uiC1fv16bGxsFGf1Q0NDOXv2LN999x1VVVWoq6tLvntD+Gvl5uZy5coVTp8+zZMnT2jSpInig03479XW1ir6Drzu4sWLBAQEsGDBAqXojSJfRP3000/4+PgoLv6uX79OQEAAVlZWLF68WPJjhTExMTx+/JiuXbuir68vWQ7hryV/npWXl/PgwQNu3bqFq6sr9vb23L59m/DwcIYNG0bTpk0lfU7Kf3dOTg4NGjQgOzub5ORkXrx4QVVVFc2bN6dHjx6SZPs9jx49YuLEiVRVVWFhYUHv3r2ZMGEC165do3HjxpIVneXqY/G5rKyMJ0+eYG5ujqamJjk5OezYsQMPDw+6du0qdbx6ITY2FkNDQ6ytrSkoKCAoKIjjx4+zefNmpXmfDwgIoFOnTordeuvWrePatWvY2dmRk5ODo6PjGz2ElEVRURETJkzg6NGjPHjwgF9//ZXg4GBevHhBYGCgojBVl9LS0li5ciUFBQV8//33BAQE4OTkxJgxYxQTiZVdQkICV69e5dy5c3Tt2pVBgwbh4OAgefE0Pz+fqVOnsmXLFl68eMHy5ct5/Pgx3377rSTDKgRBqFv1uiDl4uLC0KFDmTZtGkZGRqxatYp27drRs2dPKisrlab/hVA30tLSOHr0KLa2tpL0F3ibvL44kclk1NbWKtWd3teVlJQwdepUqqurmTp1Kj169PinC32pd6MI7wb582zdunVkZ2cjk8kIDQ1FX1+flStX0q5dO6kjKhQWFjJlyhSKi4vp2LEj7dq1o1mzZtjZ2Snl3f7g4GDc3NwIDQ3lxIkT3Lt3j4KCAg4dOkSrVq2kjqegzMVn+fMzLi6OLVu2oKmpSXl5OXZ2dnTp0oXMzEwGDhxIw4YNpY5a79y4cYM9e/YwZswY2rdvL/lNEHj1Gh8xYgQ5OTno6ekxduxYRo0aRXV1NQ8fPsTMzAw9PT2l2AkpJ3+OJiQkEBQUxLx58974flRUFB06dJAo3Stbt24lOTmZO3fuEBQUJGmWPyJfx4WGhhIcHIyWlhZWVla8//77uLq6Sv78hL//vQ8ePEhWVhYzZ85kzZo12NnZYWNjw7lz51i2bJnUMQVB+IvV24LU68e2EhISMDIyIisrS9HkXBCE/5ukpCQcHR0VO6VUVFSoqalBVVVVKRYycmVlZURHRxMZGcn9+/cpLy/H3t6ewYMHK9WFqvDuGD9+PP7+/pibmwNw5MgR0tLSmDNnDhoaGpK+fuQXAIcOHSIjI4MpU6Zw5MgRoqOjKSkpoVWrVooBEVKTZ83IyCArK4tHjx7RuXNnLC0tefz4MVlZWZJfnNYn8sdz5cqVuLq6cu/ePTIzM2nYsCHx8fFYWFiwbds2qWPWSzU1NaioqCjVjY9jx47RtGlTPD09CQoKYseOHcTHx+Pm5saoUaPw8fFRqryv++GHH7h+/TqdO3emU6dOWFhYYGZmhoqKimQ3mOS/Nz8/n23btnHs2DHmz5/PgAEDlPoG+PTp02nWrBmGhobk5ORQWVmJqqoq/fv3V5qbJEeOHOHGjRskJyczePBgPv74Y06ePElycrLSfB4JgvDXqbdNzdXU1PDx8cHHx4e8vDxCQkI4d+4cw4cPx9ramsmTJ9OpUyepYwpCvVJUVMTevXtJTEzk0aNHBAYGvrHwU8ZdUpmZmVhYWDBr1iyeP39Oeno6wcHB3L59m1atWinFnWrh3ZGWloaGhoaiGAXQt29fxo8fT2VlpeS7T+Sv54cPH+Lh4YGenh6TJk1i0qRJxMbGUlhYKGm+18mzrl69GhMTE0JDQ+nUqROZmZkYGxtjYWEhXt9/gqqqKrW1taSkpDB37lwCAwOZM2cOjRs3JigoSOws/j9Qxs/GwMBA5s6dC4C3tzf29vbU1tYSGxvL559/zuXLl/nhhx8kTvn7+vXrh729PRERERw8eBATExOsrKwYOHAg2trakmSSvx8ZGBiwYMECvLy82LBhAw4ODkozBOIflZWV0bZtW6ZPnw7A48ePuXv3LnFxcbz33nuAckxKHj58OOXl5fTo0YPevXvz4MEDdu3ahb+/v6S5BEGoG8p5a+RPatq0Kb6+vuzcuZMtW7ZgZ2dHVlaW1LEEod6Rb+svKSkhKyuLLl264O/vT2FhoWLkujKQb+xMSUlh+fLliovomJgYHjx4wJw5c/jwww8lTCi8q2xtbTE2NmbUqFEEBwdTU1PDxYsXadasGY0aNUImk0kdkaKiIp49e8aKFStYv349MTEx1NbW4urqSvfu3aWOB6B4nKKjo2nUqBFLlizBxMQEa2trQkJC2LhxI1VVVZJfSNU3FRUVDB06lNDQULS0tLC0tMTU1JSzZ88q9S4P4c9JTk6mQYMGikKJTCZj7ty56OvrM2zYMGbNmsWYMWMkTvkm+Wu+rKwMmUyGi4sL/v7+zJkzh4YNG5KZmSlZMer3dOzYkaVLlyrldL2amhoA4uPjiYiIYNGiRWRnZ2NhYUGvXr2YP3++Yhq1lM3M4dVNnKtXr6KqqoqTkxMFBQUkJCQwduxYpZ5UKgjC/069PbInCMJfJy4uDicnJ+Li4ti5c6fi4uWTTz5h4sSJkvdkkvdG8Pf3x9nZGQ8PD/bs2cPt27dxcXHBxcWlzsdCC0JlZSVRUVG4u7uzc+dOTp8+TWFhIX379qVPnz60a9dO0tfOjRs3aNu2LWVlZTx8+JAHDx6QmppKbm4utbW1eHp6MmTIEEmy/SuHDh0iNzeXJk2akJeXx6effkpkZCRHjhxR2t0dyky+G6K4uJh9+/axdu1aXFxcsLOzY+XKlVLHE/5Hfm/oz+nTp/n+++/JyMhg8eLF7N69W+KUv2/69OmYmppy48YNbG1tGThwIEVFRVhbWyvNEbP6YuTIkbi7uxMXF8eTJ09wcHCgW7duDBo0SPLdunKzZ8/GyMiIsLAwtm7dipaWFtra2jRq1EjqaIIg1JF6e2RPEIT/LfmFcnJyMo8fP0ZDQ4OOHTvSsWNHAG7duqW4WyX1rgT58Yjnz5/TokULfvzxR+zt7dmxYwffffedYoekMmxFF95+8udZZGQkp06dwtPTk+nTpzN9+nTy8vJo1KiRonGwVMWo8vJyFi1axKVLl9i0aRMODg507tyZzp07k5mZSWxsrOIIhzLIz89HJpPRr18/fvvtN3bv3s3EiRO5ffs2R44cwcPDQ+qI9U5JSQnHjx/H0NAQHx8fpk2bRr9+/UhJSRH99t4yAQEBDB06lPbt22NkZERkZCS9evUC4MKFC0o3uUy+/rh58ya6urqMGzeOpKQk2rdvz5o1a6isrOTgwYNSx6wX5J9HGRkZODg48NlnnwGQk5PDsWPH2Lp1K506dcLS0lLyjNHR0ejo6LBkyRLGjh1Ls2bN2LlzJwUFBcyaNateTC4UBOH/ThSkBEF4w+7du7G2tqZr167s27ePiIgI2rZty+TJkxU/owxFntraWry8vJgwYQK9evVi9OjRyGQyYmNjmTp1KqAcOYW3n3xxnZSURH5+PocPH8bV1RUzMzOaNm0qdTwACgoK0NbWZsCAAdTW1nLlyhXKyspwd3enX79+DBs2TGmmwp09e5awsDDOnj2Lg4MDPXr0oGPHjty6dYsrV64odk0I/xn5jtJjx46Rnp7O4MGDiYiIUPTmWr9+vTiu9xapqanhm2++ISgoCF9fX8XQH3kfodu3bzNr1iyJU75JXqi/cuUK7du3JzY2Fnd3d8aMGYOqqioeHh4YGRlJnLJ+kK97YmNjuXTpEk2aNGHEiBGYm5szY8YMZsyYIXFCFMNy0tPTsbCwYO/evbi6ugLg4ODAkSNHRDFKEN4h4sieIAgKFRUVjBo1imPHjnHgwAFiY2MZNGgQJ0+eZMqUKbRo0ULqiFRXV6Ours7GjRsZN24cOjo6lJeXU1BQwMaNGzEwMGD+/PmSHysU3g2ZmZnk5ubi5ubGiRMnSEpKIjc3F0NDQ2xsbLCwsKBTp05Kc8F/4sQJHj9+TPv27bG2tubkyZPs3bsXDw8Pvv32W6njATBu3Dg+/fRTXFxc2LhxI2pqasyYMYP09HTS0tLo0KEDurq6UsesdyZNmsTChQvJzc3l3LlzjBgxgrCwMJydnenWrZvU8YS/wOtDf7KysmjUqBFqamocPnxY6mi/KykpiQcPHnD//n2MjIz46KOPWLhwIV27dqVv375Sx6tX7t+/T1RUFAkJCWRlZWFiYoK7uzvDhg1DTU1N8vVRSUkJBQUFnDhxgtOnT/Pxxx/j5OTErl278PDwEEMWBOEdIgpSgiAoPH36lNWrV+Pk5MTFixfZunUrOjo6TJo0iZ07d0q+gJGrra3lhx9+wMLCgpEjRwKv+vekpqZiamqKgYGBKEgJdWL58uU4Ojq+8TzMyMjg+vXrJCQkoKury7JlyyRO+XeVlZUEBwezfv167O3tWbhwIWZmZuTl5SnFbq7k5GTWrl3LL7/8Ary6aBkzZgwmJibo6+sTHR3NV199JY7s/Unl5eWsXLkSU1NTTp48yY8//kirVq3w8/Nj1qxZODk5SR1R+IulpaVx9OhRbG1tlf5iPycnhyFDhmBmZoaamhq7du1SHHsW/jX5bt3KykpKS0t58OABmpqaVFZWEhsbS2RkJGvXrpW0oP/w4UOCg4M5duwY5ubmODo6cuHCBby8vMjOzqZZs2bMmTNH7JAShHeIKEgJgqAgk8k4fvw4iYmJjBgxAgsLC/bt20d6ejr+/v6SF3mio6MxMDDA1taW4uJiFi5cyIQJE4iPj+fhw4ekpqZy+PBhcVRPqDMTJ07kp59+okmTJgAsWrSIyZMnY2trS3V1NTk5OZibm0v62rl06RIFBQU4OTmRm5uLiYkJNjY27Ny5kzt37jBu3DilaRa8fv16mjdvzoABAwAICwtj7dq1+Pn5oa6uzgcffCBtwHosJiaGiIgI2rRpQ9euXTl37hy7d+9m3759UkcT3mHy98aQkBBu3rxJw4YNGTRoECYmJsTGxmJsbIyNjY3UMesF+WO5ZcsWUlNTSU9P57PPPsPd3Z3y8nIAdHV1Je2vOXv2bEXD/WfPnhEXF8fhw4cxNzdnzZo1mJiYSJJLEATpiB5SgiAArxYyeXl5ODs7M3jwYNTU1IiMjKS0tFTRe0JqISEh3LhxA1NTUwYPHkyTJk3YvHkzDg4O9O7dm5kzZ6KioqLomSIIf6XQ0FCsra0Vxaj8/HweP36sGKetrq6Oubk5IF0zc3g1NfO3336jX79+uLi4cOzYMR48eEDLli2JjY2lpqZGaQpS8mbMHTp0UDRjnj17tqIQJXVRvL46duwYbdq0YcaMGTRo0IDLly+Tm5vLzJkzpY4mvONUVVXJz89nxYoVfPzxx6Snp7Nw4UKMjY1xd3fHzc1N6oj1hqqqKmVlZVy5coWAgADGjBmDjY0NwcHBFBYWMnz4cEC6/prJycmUlpYyZ84cAOzs7OjYsSOjR49m0aJFPH36FBMTEzGQRhDeMaIgJQjvOHnxZu/evSQlJfHw4UM0NDRwcXGhc+fOmJiYYGVlBUh7UV1bW8uMGTPo168fqampnDp1iuzsbLKyspg0aRJdunR54/9HEP5qAQEBtG/fXvHfYWFhtGzZEjU1NUWvM2Xg6+uLmpoagYGBGBkZ8f3331NeXs69e/f4+OOPlWa63r9qxjxt2jTFz4hi1H/u9cllgYGBNG/enNzcXH755RecnZ3x9fUVx6AESd27dw9bW1tSU1Px9fVl/PjxFBUVkZ2dzc2bN0lKSlKa/nvKTv56v3HjBi1btqS0tBRjY2OMjY1xdHRk5cqV+Pr6SpoxKCiIIUOGAK+Oj8s1btwYT09PgoODcXFxEcUoQXjHiCN7giAAMG3aNObNm8emTZuws7MjNjaW5ORkRo4cyaxZs5RmZ8KFCxdo0KABLi4upKamEh4eTnx8PDo6OmzatEnqeMI7oqamBn9/f65evYqmpib9+/cnPDyclStXKgq4yiY1NZWzZ8/StGlTRZFKWb3ejPnx48dYW1szefJkOnXqJHW0ekP+nr1o0SI+/PBDmjZtyr59+3jx4gXa2tpYW1szevRoqWMK7zBfX1+Ki4tp0aIFVlZWTJ48WbHjtLq6msrKSrS1taUNWc9kZmaye/du4uLi6NGjB9OnT+fIkSPExcXxzTffSLqWc3FxYejQofj5+WFoaPjG93bu3EleXh7z5s2TJJsgCNJRjtu3giBI6uHDh1RUVGBoaEhOTg7ff/89cXFxFBYW4unpCUi3xVtOvoX7/v37dOvWDX19fdzc3HB2diY3NxeZTAaIHVJC3VBTU+PLL7+ktLSU8PBwzpw5Q3JyMosXL8bHx4dBgwYpxYXUo0ePKCgowNTUlBYtWuDl5cWePXsIDw9nyJAhdO3aVSmbx8qLZr6+vqSlpXHo0CGysrKkjlWvqKqqUltbi6qqKhERESQkJNC7d2+GDx/Od999h76+vtQRhXfcwYMHiY6O5syZM1y8eJHr16/Tq1cvevfuTbNmzZRml6myq6ys5P79+wQEBGBmZoazszMRERE8e/aMiRMnoqqqyty5cyXN+PoO2OHDh2NqasqAAQMYOHAgOjo6xMfHM2PGDEkzCoIgDbFDShAECgsLuXz5MhoaGoSGhrJ69WpSUlL48ccf2bJli9TxFNLT0+nTpw9OTk58/vnnYtKWoFRyc3MJCQnh0KFDNG/enB9++EHSPLdu3WLRokW0atWKxMREAHr27El5eTmnT5+mqqqKkydPiiayb7m7d+/y888/Y29vz+zZs0lLS2PhwoXs3r1bHNkTJPN7x5qvXbvG0aNHiYyMpFu3bnz77bcSpatfduzYwe3bt7GysqKyspKCggKuXr2KjY0Nf/vb3zA3N8fU1FTqmAp5eXkEBwdz7tw5srKyaNKkCaqqqhw+fFjqaIIgSEAUpARBeMO8efO4du0adnZ29OnTh9GjRyvFriN5hkePHnH48GHFwqVHjx7MmjULMzMzSfMJwutKSkrQ1dWV/LVTUlJCcXEx6urq3L17l8zMTIyMjKipqeHu3buS3zUX/hpJSUnIZDL09fV5/vw5GhoaaGpqEhsby+HDh+nbty/jxo2TOqYg4O/vz4sXL9DQ0MDLywsPDw9qa2vJzMzEwcFB6nj1wsiRI1m/fj1GRkbAq/XSjRs32Lx5M3/7299wc3NTmrYL/ygtLY2jR49iY2OjaLouCMK7RRSkBOEdJV+c5OTkcP36dU6dOsWUKVPo2LEj0dHRvHz5Eg8PD6U6zlNYWEhFRQXGxsYA3L59m9WrV+Pt7c3YsWPFZBZBEN55iYmJDBs2jMaNG6Orq4uTkxP37t0jLy+Pfv36cePGDZYuXaoYBCEIdU2+/oiJiWH58uXMnj2bJ0+ecO/ePUpKSjA1NeXzzz9XqvWHsgoNDeXKlSssW7aMsrIyGjRooNh5tnPnTgoKCpg1a5Z4LAVBUFricLYgvOPWrl1Lu3btqKmpITExESsrK2QyGV27dpU6GvDmwnXDhg3IZDJMTU0V46DHjx9P9+7dAen7XAlCfSGKt2+n2tpazM3N6devH++99x5jxozB0tKS+Ph4vv/+e5YsWSKO6QmSk+/UKS4uZuHChXTp0oXCwkJycnJIS0tTFFaEf+/1aa9aWlrAq55SGhoauLq6smXLFvFYCoKg1JRv76YgCHVCVVWV8vJyHj9+zNChQ9HV1aVHjx4YGhpy6tQpcnJypI74hgMHDjB9+nQcHR15/vw5R48eZfbs2QQHByua9wqC8J8Rxai3k4qKCk2aNMHPz4+UlBRmzZpFamoqhw4dok+fPmhqalJVVSV1TOEdVlpaSlpaGjKZjOXLlxMQEMDjx49p0qQJDg4O+Pj4MGDAAKlj1gs1NTXY2tpy4sQJBg4cyIYNG8jKykJDQwOA8+fPKwbT1NTUSBlVEAThXxIFKUF4hz158gRnZ2cSExPR1dWlWbNmlJeXk5ycTNOmTaWOB7wqnNXU1FBYWEinTp1IT09n3bp1bN++nR49ejB//nwAUZASBEH4/2xtbdm5cyf9+vVj8+bNxMTEMGbMGACxW0KQ1KlTp4iIiEBVVZWlS5dSW1tLr169GDRoEIcOHUImkykKKsIfk097PX78uKL4PGbMGMaMGcO+ffuIj4+nb9++ip8VBEFQRuLIniC8w2xsbKiurmbEiBG4u7vz6NEj9uzZQ5s2bVBVVZW8CWZUVBRaWlro6urSrl079u7dS+PGjSkqKsLExISUlBTF6HJlbNYpCIIgBfl79/Dhw9m2bRvh4eEcPXqUAQMGiIt9QVKXLl1i3rx5wKupn3Z2dtTW1pKQkMAXX3xBVFSU5BNK6xsdHR28vb3x9vYmLy+PS5cucejQIQwNDdHT05N8LScIgvBHRFNzQXjHVFZWUlRUhJqaGgYGBgBER0dz/PhxYmNjGTFiBL169cLS0lLyRUzfvn2pqKhg8uTJWFpaoqenR1BQEKGhoTRs2JC2bduyZMkSyXMKgiAos8jISDZs2MAXX3xBy5YtpY4jvKOSk5P56aef2LJlC/CqcDp8+HB27NhBkyZN2LhxI507d8bFxUXipG8HZZn2KgiC8EdEQUoQ3jEBAQFcunSJnJwcli1bRrNmzYiPj8fBwYEWLVooVbPjhIQEVq1aRXFxMU5OTujo6KClpUWrVq0oLS2lU6dOWFhYiIKUIAjCH6itrSUlJQUzMzMaN24sdRzhHbV+/XpsbGzo378/8GpC3OnTp/n+++/JyMhg8eLF7N69W+KUgiAIQl0SR/YE4R1z5swZtmzZQnx8PHv27MHQ0BB1dXUCAwOZNm2aUt2ZbNOmDcuXL+fw4cM0b94cNzc37t27R0hICFZWVlhYWADiuJ4gCMIfUVFRwdHRUeoYwjsuICCAoUOH0r59e4yMjIiMjKRXr14AXLhwAXd3d4kTCoIgCHVNFKQE4R0SGhqKs7MzhoaGtGjRgrt373Lx4kVKS0sJDg7mwIEDODg4oK2tLXVUBQcHByZNmsQPP/xAYmIin376KT4+Pjx58gRA7I4SBEEQBCVXU1PDN998Q1BQEL6+vhgZGZGVlcX06dMBuH37NrNmzZI4pSAIglDXxFWcILxDAgICFNPzrl+/zrhx49DQ0EBfXx9nZ2eKioqUohhVXl7O8+fPART/9Pf3R1VVla+++ori4mKsrKwAsTtKEARBEJSdmpoaPj4+rF27lkOHDjF06FDs7Oz48MMPGTp0KE+fPsXe3l7qmIIgCEIdEz2kBOEdUVNTg7+/P1evXkVbW5vs7Gx++uknOnXqBMCaNWuwtrZmxIgRkjfAXLRoEfHx8ejp6dG5c2fu3LlDVlYWrVq14uzZs7i6uhIQECBZPkEQBEEQ/u/S0tI4evQotra2DBs2TOo4giAIQh0TBSlBeMeUlpYSERHB+fPniYuLw8zMDB8fHwIDA9m8eTN6enqS5qupqWHp0qVkZGRQWFhIixYtmD17Nnp6epSVlWFiYkJhYSEGBgaSF84EQRAEQRAEQRCE/44oSAnCOywvL49Lly5x6NAhDA0N2bZtm9L0ZHrx4gV3797l8uXL3Llzh+bNm+Pp6UmXLl3Q0tKSOp4gCIIgCIIgCILwfyAKUoIgAFBSUoKurq5S7jrKzc0lMjKSCxcuYG1tzYIFC6SOJAiCIAiCIAiCIPwfiIKUIAj1hkwmo6ysDB0dHaXZySUIgiAIgiAIgiD8eaIgJQiCIAiCIAiCIAiCINQpsb1AEARBEARBEARBEARBqFOiICUIgiAIgiAIgiAIgiDUKVGQEgRBEARBEARBEARBEOqUutQBBEEQBEGof2pra9m5cycHDx6kqqoKFRUVunTpwueff87XX3+NlZUVfn5+UscUBEEQBEEQlJTYISUIgiAIwp/2/fffc/bsWQICArh06RKnTp2iqqqKqVOnIualCIIgCIIgCP+OmLInCIIgCMKfUlhYiJeXF8ePH8fW1lbx9YqKCsLDwzl//jzNmjXDz8+PuLg4Vq5cycuXL1FVVWXJkiV4eHhQXV3N8uXLiY6ORiaT4eDgwKpVq9DU1Pzdr+vq6kr4fywIgiAIgiD8r4kdUoIgCIIg/CkJCQmYmJi8UYwCaNiwId27d0dV9e/Li6VLlzJp0iTOnz/P1KlTWbZsGQDXrl0jMzOT8+fPExQUhJ2dHXFxcf/y64IgCIIgCMLbRfSQEgRBEAThT3nx4gWGhob/0c+eOHECFRUVANzc3MjMzATAwMCAtLQ0Ll68SJcuXZgzZw4At27d+t2vC4IgCIIgCG8XsUNKEARBEIQ/xcTEhJycnP/oZ0+fPs3w4cPp3bs3H3/8saK/VOvWrVmyZAm7d++mc+fOfPbZZxQXF//LrwuCIAiCIAhvF1GQEgRBEAThT3F0dKS4uJg7d+688fWqqip++uknysrKAMjJyWHJkiV88803XLhwgW3btr3x83369GH37t1cvnyZsrIyfv311z/8uiAIgiAIgvD2EAUpQRAEQRD+FF1dXaZOncrChQt59OgRAGVlZSxdupSkpCS0tLQAyM/PR1tbm+bNm1NdXc3BgwcBKCkp4ejRo/z8888ANGnSBBsbG4B/+XVBEARBEATh7SJ6SAmCIAiC8KdNnToVTU1NZsyYQU1NDWpqanTv3p3ly5crGpc7Ojri5eVF9+7dMTU1ZeHChcTGxvLRRx/x22+/8cUXX+Dt7Y2amhrW1tasWrUK4F9+XRAEQRAEQXh7qNTKmzkIgiAIgiAIgiAIgiAIQh0QR/YEQRAEQRAEQRAEQRCEOiUKUoIgCIIgCIIgCIIgCEKdEgUpQRAEQRAEQRAEQRAEoU6JgpQgCIIgCIIgCIIgCIJQp0RBShAEQRAEQRAEQRAEQahToiAlCIIgCIIgCIIgCIIg1ClRkBIEQRAEQRAEQRAEQRDqlChICYIgCIIgCIIgCIIgCHVKFKQEQRAEQRAEQRAEQRCEOvX/AL7DZY5u4YE0AAAAAElFTkSuQmCC
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>We can see from the plot above that some covenants:</p>
<ol>
<li>Are not seen at all</li>
<li>Suboptimal covenants tend to fall lower in the spec rankings, but this may not be entirely accurate, as high end players are more likely to select the best option already, and some covenant abilities can find niche uses.</li>
</ol>
<p>Speaking of imbalance, let's focus back on dungeon performance.</p>

</div>
</div>
</div>
</body>


</html>
