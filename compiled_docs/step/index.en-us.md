{"meta":"","api":"<h2 id=\"API\">API <a class=\"header-anchor scroll-count-item\" href=\"#API\" data-scroll-id=\"API\">#</a></h2>\n<h3 id=\"Step\">Step <a class=\"header-anchor scroll-count-item\" href=\"#Step\" data-scroll-id=\"Step\">#</a></h3>\n<table>\n<thead>\n<tr>\n<th>Param</th>\n<th>Descripiton</th>\n<th>Type</th>\n<th>Default Value</th>\n</tr>\n</thead>\n<tbody>\n<tr>\n<td>current</td>\n<td>current step</td>\n<td>Number</td>\n<td>0</td>\n</tr>\n<tr>\n<td>shape</td>\n<td>shape<br><br><strong>optional</strong>:<br>'circle', 'arrow', 'dot'</td>\n<td>Enum</td>\n<td>'circle'</td>\n</tr>\n<tr>\n<td>direction</td>\n<td>dispaly direction<br><br><strong>optional</strong>:<br>'horizontal', 'vertical'</td>\n<td>Enum</td>\n<td>'horizontal'</td>\n</tr>\n<tr>\n<td>labelPlacement</td>\n<td>Content arrangement in horizontal layout<br><br><strong>optional</strong>:<br>'horizontal', 'vertical'</td>\n<td>Enum</td>\n<td>'vertical'</td>\n</tr>\n<tr>\n<td>readOnly</td>\n<td>enable read-only mode</td>\n<td>Boolean</td>\n<td>-</td>\n</tr>\n<tr>\n<td>animation</td>\n<td>enable animation</td>\n<td>Boolean</td>\n<td>true</td>\n</tr>\n<tr>\n<td>itemRender</td>\n<td>custom node render function <br><br><strong>Function signature</strong>:<br>Function(index: Number, status: String) =&gt; Node</td>\n<td>Function</td>\n<td>-</td>\n</tr>\n<tr>\n<td>stretch</td>\n<td>stretch width of step item</td>\n<td>Boolean</td>\n<td>false</td>\n</tr>\n</tbody>\n</table>\n<h3 id=\"Step Item\">Step.Item <a class=\"header-anchor scroll-count-item\" href=\"#Step Item\" data-scroll-id=\"Step Item\">#</a></h3>\n<table>\n<thead>\n<tr>\n<th>Param</th>\n<th>Descripiton</th>\n<th>Type</th>\n<th>Default Value</th>\n</tr>\n</thead>\n<tbody>\n<tr>\n<td>status</td>\n<td>The status of a step, if not passed, is generated based on the current attribute of the outer Step, with optional values <code>wait</code>, <code>process</code>, <code>finish</code><br><br><strong>optional</strong>:<br>'wait', 'process', 'finish'</td>\n<td>Enum</td>\n<td>-</td>\n</tr>\n<tr>\n<td>title</td>\n<td>title</td>\n<td>ReactNode</td>\n<td>-</td>\n</tr>\n<tr>\n<td>percent</td>\n<td>percent</td>\n<td>Number</td>\n<td>-</td>\n</tr>\n<tr>\n<td>icon</td>\n<td>icon</td>\n<td>String</td>\n<td>-</td>\n</tr>\n<tr>\n<td>content</td>\n<td>Content for vertical content filling</td>\n<td>ReactNode</td>\n<td>-</td>\n</tr>\n<tr>\n<td>disabled</td>\n<td>disable step node</td>\n<td>Boolean</td>\n<td>-</td>\n</tr>\n<tr>\n<td>itemRender</td>\n<td>custom node render function (it will overwirde Step's itemRender)<br><strong>Function signature</strong>:<br>Function(index: Number, status: String) =&gt; Node</td>\n<td>Function</td>\n<td>-</td>\n</tr>\n<tr>\n<td>onClick</td>\n<td>the callback when click to step node <br><br><strong>Function signature</strong>:<br>Function(index: Number) =&gt; void<br><strong>Parameters</strong>:<br><em>index</em>: {Number} node index</td>\n<td>Function</td>\n<td>() =&gt; { }</td>\n</tr>\n</tbody>\n</table>\n"}