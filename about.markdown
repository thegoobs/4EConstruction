---
title: About Us
order: 2
layout: page
---

4E Construction Services provides a full range of construction services on public works and private development Projects.  We have extensive experience and knowledge of the Central Texas area.  Since the inception of 4E in 2012, we have completed Projects in and around the South Austin, San Marcos, Bastrop, Kyle, Georgetown, Niederwald, Wimberley, and Buda areas.

The 4E Construction Team has over 50 years of construction and engineering experience.  Previously completed Projects include water and wastewater plants, pump and lift stations, and related facilities.  Other Projects completed under previous engagements include public works projects, parks, utility infrastructure, new subdivisions, and marinas. 
 We have earned a solid reputation with our Clients and peers by maintaining our motto:  To complete each Project in an efficient and timely manner.

### Many of the Projects Completed Include:

* Shepherd Mountain Pump Station
* Southeast, Northeast and East Metropolitan Parks
* The Steiner Ranch Wastewater Treatment Plant

 and many others in Central Texas.

<hr/>
<br/>
<h1 style="text-align: center;">About the Team</h1>
<div class="employee-container">
	{% assign employees = site.employees | sort: 'order' %}
	{% for employee in employees %}
		<div class="employee-entry">
			<h2 class="employee-title">
				{{employee.title}}
			</h2>
			<h4 class="employee-subtitle">
				{{employee.position}}
			</h4>
			<p>
				{{employee.phone}}
			</p>
			<a href="mailto:{{employee.Email}}">
				{{employee.email}}
			</a>
			<p>
				{{employee.content}}
			</p>
			<h4>
				Education
			</h4>
			<p>
				{{employee.education}}
			</p>
			{% if employee.licenses %}
				<h4>
					Licenses
				</h4>
				<ul>
				{% for i in employee.licenses %}
					<li>
						{{i}}
					</li>
				{% endfor %}
				</ul>
			{% endif %}
		</div>
		<hr/>
		<br/>
	{% endfor %}
</div>