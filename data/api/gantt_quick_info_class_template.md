quick_info_class
=============

@short:specifies the CSS class that will be applied to  the pop-up edit form

@params: 
- start		Date		the date when a task is scheduled to begin
- end		Date		the date when a task is scheduled to be completed
- task		object		the task object


@example:
gantt.templates.quick_info_class = function(start, end, task){ 
	return task.type == gantt.config.types.milestone ? "milestone_popup" : "";
};

@template:	api_template
@descr:

{{note This template is defined in the **ext/dhtmlxgantt_quick_info.js** extension, so you need to include it on the page.}}



@related:
desktop/touch_templates.md