---
title: Ticket Replies API Reference
has_superbar: Yes
route_path: /wpas-api/v1/tickets/<ticket_id>/replies
resource: Ticket Reply
---

<section class="route">
	<div class="primary">
		{% include reference-parts/schema.html schema=site.data.ticket_reply.schema %}
	</div>
	<div class="secondary">
		<h3>Example Request</h3>

		<code>$ curl -X OPTIONS -i http://demo.getawesomesupport.com/wp-json{{ site.data.ticket_reply.routes[page.route_path].nicename }}</code>
	</div>
</section>

{% assign route=site.data.ticket_reply.routes['/wpas-api/v1/tickets/<ticket_id>/replies'] %}
{% include reference-parts/list-item.html route=route %}

{% assign route=site.data.ticket_reply.routes['/wpas-api/v1/tickets/<ticket_id>/replies/<id>'] %}
{% include reference-parts/get-item.html route=route %}

{% assign route=site.data.ticket_reply.routes['/wpas-api/v1/tickets/<ticket_id>/replies'] %}
{% include reference-parts/create-item.html route=route %}

{% assign route=site.data.ticket_reply.routes['/wpas-api/v1/tickets/<ticket_id>/replies/<id>'] %}
{% include reference-parts/update-item.html route=route %}

{% assign route=site.data.ticket_reply.routes['/wpas-api/v1/tickets/<ticket_id>/replies/<id>'] %}
{% include reference-parts/delete-item.html route=route %}
