# @trigger

Use the `@trigger` decorator to trigger a flow [deployed on Argo Workflows](/production/scheduling-metaflow-flows/scheduling-with-argo-workflows) based on an external event.

Read more in [Triggering Flows Based on External Events](/production/event-triggering/external-events).

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! Instead, edit the notebook w/the location & name as this file. -->


<DocSection type="decorator" name="trigger" module="metaflow" show_import="True" heading_level="3" link="https://github.com/Netflix/metaflow/tree/master/metaflow/plugins/events_decorator.py#L14">
<SigArgSection>
<SigArg name="..." />
</SigArgSection>
<Description summary="Specifies the event(s) that this flow depends on." extended_summary="```\n@trigger(event='foo')\n```\nor\n```\n@trigger(events=['foo', 'bar'])\n```\n\nAdditionally, you can specify the parameter mappings\nto map event payload to Metaflow parameters for the flow.\n```\n@trigger(event={'name':'foo', 'parameters':{'my_param': 'event_field'})\n```\nor\n```\n@trigger(events=[{'name':'foo', 'parameters':{'my_param_1': 'event_field_1'},\n                 {'name':'bar', 'parameters':{'my_param_2': 'event_field_2'}])\n```" />
<ParamSection name="Parameters">
	<Parameter name="event" type="Union[str, dict], optional" desc="Event dependency for this flow." />
	<Parameter name="events" type="List[Union[str, dict]], optional" desc="Events dependency for this flow." />
	<Parameter name="options" type="dict, optional" desc="Backend-specific configuration for tuning eventing behavior." />
</ParamSection>
</DocSection>
