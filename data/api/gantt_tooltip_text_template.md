tooltip_text
=============

@short:specifies the text of tooltips

@require:tooltip

@params: 
- start	Date	the date when a task is scheduled to begin
- end	Date	the date when a task is scheduled to be completed
- task	object	the task object

@example:
gantt.templates.tooltip_text = function(start,end,task){
	return "<b>Task:</b> "+task.text+"<br/><b>Start date:</b> " + 
    gantt.templates.tooltip_date_format(start)+ 
    "<br/><b>End date:</b> "+gantt.templates.tooltip_date_format(end);
};

@template:	api_template

@returns:
- text		string		html text which will be rendered in the gantt

@descr:

{{note This template is defined in the **ext/dhtmlxgantt_tooltip.js** extension, so you need to include it on the page. Read the details in the desktop/tooltips.md article.}}




@relatedapi:
	 api/gantt_tooltip_date_format_template.md
@related:
	desktop/tooltip_templates.md
	desktop/tooltips.md
