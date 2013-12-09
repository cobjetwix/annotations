<h1>Annotations - Highcharts module</h1>

<h2>Sample code</h2>

<pre><code>new Highcharts.Chart({
  chart: {
    renderTo: container
  },
  series: [{
      data: [29.9, 71.5, 106.4, 129.2, 144.0, 176.0]
  }],
  annotations: [{
    xValue: 4,
    yValue: 125,
    title: {
        text: "Annotated chart!"
    }
  }]
})
</code></pre>

<h2>Available options</h2>

<h3>Chart options</h3>

<table>
<thead>
<tr>
<th align="left">Option            </th>
<th align="left"> Description</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">chart.annotations </td>
<td align="left"> Array containing annotation configuration objects</td>
</tr>
</tbody>
</table>


<h3>Annotation configuration object</h3>

<table>
<thead>
<tr>
<th align="left">Option                                    </th>
<th align="left"> Description</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">x<br>y                                    </td>
<td align="left"> Annotation position defined in pixels</td>
</tr>
<tr>
<td align="left">xValue<br>yValue                          </td>
<td align="left"> Annotation position defined using axis values</td>
</tr>
<tr>
<td align="left">xAxis<br>yAxis                            </td>
<td align="left"> Axis index, default to 0</td>
</tr>
<tr>
<td align="left">anchorX<br>anchorY                        </td>
<td align="left"> Defines annotation anchor point (see below), available values:<br>anchorX: left, center, right<br>anchorY: top, middle, bottom</td>
</tr>
<tr>
<td align="left">allowDragX<br>allowDragY</td>
<td align="left"> Allow user to drag and drop an annotation. Horizontal and vertical.</td>
</tr>
<tr>
<td align="left">linkedTo                                  </td>
<td align="left"> Link annotation to point or series using it's id</td>
</tr>
<tr>
<td align="left">title                                     </td>
<td align="left"> Title configuration object</td>
</tr>
<tr>
<td align="left">title.text                                </td>
<td align="left"> Title text</td>
</tr>
<tr>
<td align="left">title.x<br>title.y                        </td>
<td align="left"> Title position in pixels, relative to annotation position</td>
</tr>
<tr>
<td align="left">title.style                               </td>
<td align="left"> Additional CSS styles for title</td>
</tr>
<tr>
<td align="left">title.style.color                         </td>
<td align="left"> Title text color</td>
</tr>
<tr>
<td align="left">title.style.fontSize                      </td>
<td align="left"> Title font size</td>
</tr>
<tr>
<td align="left">shape                                     </td>
<td align="left"> Shape configuration object</td>
</tr>
<tr>
<td align="left">shape.type                                </td>
<td align="left"> Shape type, available types are "path", "circle" and "rect"</td>
</tr>
<tr>
<td align="left">shape.units                               </td>
<td align="left"> Defines whether shape uses pixels or axis values</td>
</tr>
<tr>
<td align="left">shape.params                              </td>
<td align="left"> Shape parameters (parameters are passed to renderer method like rect, circle or path)</td>
</tr>
</tbody>
</table>


<h3>Available shape parameters</h3>

<table>
<thead>
<tr>
<th align="left">Option                                      </th>
<th align="left"> Description                                        </th>
<th align="left"> Limited to</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">shape.params.x<br>shape.params.y             </td>
<td align="left"> Shape position relative to the annotation position </td>
<td align="left">rect<br>circle</td>
</tr>
<tr>
<td align="left">shape.params.width<br>shape.params.height    </td>
<td align="left"> Rectangle width and height (only for "rect" type)  </td>
<td align="left"> rect</td>
</tr>
<tr>
<td align="left">shape.params.d                               </td>
<td align="left"> Path definition (only for "path" type)             </td>
<td align="left"> path</td>
</tr>
<tr>
<td align="left">shape.params.r                               </td>
<td align="left"> Circle radius                                      </td>
<td align="left"> circle</td>
</tr>
<tr>
<td align="left">shape.params.fill                            </td>
<td align="left"> Fill color, default: transparent                   </td>
<td align="left"> -</td>
</tr>
<tr>
<td align="left">shape.params.stroke                          </td>
<td align="left"> Stroke color, default: black                       </td>
<td align="left"> -</td>
</tr>
<tr>
<td align="left">shape.params.strokeWidth                     </td>
<td align="left"> Stroke width (and line width for path), default: 2 </td>
<td align="left"> -</td>
</tr>
</tbody>
</table>


<h3>Chart.annotations</h3>

<table>
<thead>
<tr>
<th align="left">Property                       </th>
<th align="left"> Description</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">chart.annotations.add(options) </td>
<td align="left"> Add one annotation with given options</td>
</tr>
<tr>
<td align="left">chart.annotations.redraw()     </td>
<td align="left"> Redraw all annotations</td>
</tr>
<tr>
<td align="left">chart.annotations.allItems     </td>
<td align="left"> Array containing all annotations</td>
</tr>
</tbody>
</table>


<h3>Annotation object</h3>

<table>
<thead>
<tr>
<th align="left">Property                   </th>
<th align="left"> Description</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">annotation.update(options) </td>
<td align="left"> Update annotation with given options</td>
</tr>
<tr>
<td align="left">annotation.destroy()       </td>
<td align="left"> Destroy annotation</td>
</tr>
</tbody>
</table>



<h2>Advanced demo</h2>


<div>Go to project page to see this module in action: http://blacklabel.github.io/annotations/</div>

