{"title":"内容回填","meta":{"title":"内容回填","description":"\n<p>提醒: <code>https://www.easy-mock.com/mock/5b713974309d0d7d107a74a3/alifd/upload</code>接口:</p>\n<blockquote>\n<ol>\n<li>该接口仅作为测试使用,业务请勿使用</li>\n</ol>\n</blockquote>\n<blockquote>\n<ol start=\"2\">\n<li>该接口仅支持图片上传,其他文件类型接口请自备</li>\n</ol>\n</blockquote>\n","order":"6"},"codes":{"jsx":"import { Upload, Button, Field, Form } from '@alifd/next';\n\nconst FormItem = Form.Item;\n\nconst value = [{\n    name: 'pic.png',\n    fileName: 'pic.png',\n    state: 'done',\n    size: 1000,\n    downloadURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg',\n    fileURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg',\n    imgURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg'\n}];\n\nclass App extends React.Component {\n\n    field = new Field(this);\n\n    setValues = () => {\n        this.field.setValues({\n            upload: [...value]\n        });\n    };\n\n    getValues = () => {\n        const values = this.field.getValues();\n        console.log(values);\n    };\n\n    render() {\n\n        return (\n            <Form field={this.field}>\n                <FormItem required>\n                    <Upload\n                        listType=\"text\"\n                        name=\"upload\"\n                        action=\"https://www.easy-mock.com/mock/5b713974309d0d7d107a74a3/alifd/upload\"\n                        defaultValue={value}\n                    >\n                        <Button>Upload</Button>\n                    </Upload>\n                </FormItem>\n                <div>\n                    <Button onClick={this.setValues} type=\"primary\" style={{margin: '0 0 10px'}}>Set Data</Button>&nbsp;&nbsp;\n                    <Button onClick={this.getValues} type=\"primary\" style={{margin: '0 0 10px'}}>Get Data</Button>&nbsp;&nbsp;\n                    <Button onClick={() => this.field.reset()} type=\"primary\" style={{margin: '0 0 10px'}}>Reset</Button>&nbsp;&nbsp;\n                    <Button onClick={() => this.field.validate()} type=\"primary\" style={{margin: '0 0 10px'}}>Validate</Button>\n                </div>\n            </Form>\n        );\n    }\n}\n\nReactDOM.render(<App />, mountNode);\n"},"body":"\n\n````jsx\nimport { Upload, Button, Field, Form } from '@alifd/next';\n\nconst FormItem = Form.Item;\n\nconst value = [{\n    name: 'pic.png',\n    fileName: 'pic.png',\n    state: 'done',\n    size: 1000,\n    downloadURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg',\n    fileURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg',\n    imgURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg'\n}];\n\nclass App extends React.Component {\n\n    field = new Field(this);\n\n    setValues = () => {\n        this.field.setValues({\n            upload: [...value]\n        });\n    };\n\n    getValues = () => {\n        const values = this.field.getValues();\n        console.log(values);\n    };\n\n    render() {\n\n        return (\n            <Form field={this.field}>\n                <FormItem required>\n                    <Upload\n                        listType=\"text\"\n                        name=\"upload\"\n                        action=\"https://www.easy-mock.com/mock/5b713974309d0d7d107a74a3/alifd/upload\"\n                        defaultValue={value}\n                    >\n                        <Button>Upload</Button>\n                    </Upload>\n                </FormItem>\n                <div>\n                    <Button onClick={this.setValues} type=\"primary\" style={{margin: '0 0 10px'}}>Set Data</Button>&nbsp;&nbsp;\n                    <Button onClick={this.getValues} type=\"primary\" style={{margin: '0 0 10px'}}>Get Data</Button>&nbsp;&nbsp;\n                    <Button onClick={() => this.field.reset()} type=\"primary\" style={{margin: '0 0 10px'}}>Reset</Button>&nbsp;&nbsp;\n                    <Button onClick={() => this.field.validate()} type=\"primary\" style={{margin: '0 0 10px'}}>Validate</Button>\n                </div>\n            </Form>\n        );\n    }\n}\n\nReactDOM.render(<App />, mountNode);\n````","html":"<script>(function(){'use strict';\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _next = require('@alifd/next');\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\nvar FormItem = _next.Form.Item;\n\nvar value = [{\n    name: 'pic.png',\n    fileName: 'pic.png',\n    state: 'done',\n    size: 1000,\n    downloadURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg',\n    fileURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg',\n    imgURL: 'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg'\n}];\n\nvar App = function (_React$Component) {\n    _inherits(App, _React$Component);\n\n    function App() {\n        var _ref;\n\n        var _temp, _this, _ret;\n\n        _classCallCheck(this, App);\n\n        for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {\n            args[_key] = arguments[_key];\n        }\n\n        return _ret = (_temp = (_this = _possibleConstructorReturn(this, (_ref = App.__proto__ || Object.getPrototypeOf(App)).call.apply(_ref, [this].concat(args))), _this), _this.field = new _next.Field(_this), _this.setValues = function () {\n            _this.field.setValues({\n                upload: [].concat(value)\n            });\n        }, _this.getValues = function () {\n            var values = _this.field.getValues();\n            console.log(values);\n        }, _temp), _possibleConstructorReturn(_this, _ret);\n    }\n\n    _createClass(App, [{\n        key: 'render',\n        value: function render() {\n            var _this2 = this;\n\n            return React.createElement(\n                _next.Form,\n                { field: this.field },\n                React.createElement(\n                    FormItem,\n                    { required: true },\n                    React.createElement(\n                        _next.Upload,\n                        {\n                            listType: 'text',\n                            name: 'upload',\n                            action: 'https://www.easy-mock.com/mock/5b713974309d0d7d107a74a3/alifd/upload',\n                            defaultValue: value\n                        },\n                        React.createElement(\n                            _next.Button,\n                            null,\n                            'Upload'\n                        )\n                    )\n                ),\n                React.createElement(\n                    'div',\n                    null,\n                    React.createElement(\n                        _next.Button,\n                        { onClick: this.setValues, type: 'primary', style: { margin: '0 0 10px' } },\n                        'Set Data'\n                    ),\n                    '\\xA0\\xA0',\n                    React.createElement(\n                        _next.Button,\n                        { onClick: this.getValues, type: 'primary', style: { margin: '0 0 10px' } },\n                        'Get Data'\n                    ),\n                    '\\xA0\\xA0',\n                    React.createElement(\n                        _next.Button,\n                        { onClick: function onClick() {\n                                return _this2.field.reset();\n                            }, type: 'primary', style: { margin: '0 0 10px' } },\n                        'Reset'\n                    ),\n                    '\\xA0\\xA0',\n                    React.createElement(\n                        _next.Button,\n                        { onClick: function onClick() {\n                                return _this2.field.validate();\n                            }, type: 'primary', style: { margin: '0 0 10px' } },\n                        'Validate'\n                    )\n                )\n            );\n        }\n    }]);\n\n    return App;\n}(React.Component);\n\nReactDOM.render(React.createElement(App, null), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> Upload<span class=\"token punctuation\">,</span> Button<span class=\"token punctuation\">,</span> Field<span class=\"token punctuation\">,</span> Form <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> FormItem <span class=\"token operator\">=</span> Form<span class=\"token punctuation\">.</span>Item<span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> value <span class=\"token operator\">=</span> <span class=\"token punctuation\">[</span><span class=\"token punctuation\">{</span>\n    name<span class=\"token operator\">:</span> <span class=\"token string\">'pic.png'</span><span class=\"token punctuation\">,</span>\n    fileName<span class=\"token operator\">:</span> <span class=\"token string\">'pic.png'</span><span class=\"token punctuation\">,</span>\n    state<span class=\"token operator\">:</span> <span class=\"token string\">'done'</span><span class=\"token punctuation\">,</span>\n    size<span class=\"token operator\">:</span> <span class=\"token number\">1000</span><span class=\"token punctuation\">,</span>\n    downloadURL<span class=\"token operator\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg'</span><span class=\"token punctuation\">,</span>\n    fileURL<span class=\"token operator\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg'</span><span class=\"token punctuation\">,</span>\n    imgURL<span class=\"token operator\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB19O79MVXXXXcZXVXXXXXXXXXX-1024-1024.jpg'</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">class</span> <span class=\"token class-name\">App</span> <span class=\"token keyword\">extends</span> <span class=\"token class-name\">React<span class=\"token punctuation\">.</span>Component</span> <span class=\"token punctuation\">{</span>\n\n    field <span class=\"token operator\">=</span> <span class=\"token keyword\">new</span> <span class=\"token class-name\">Field</span><span class=\"token punctuation\">(</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function-variable function\">setValues</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">.</span><span class=\"token function\">setValues</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span>\n            upload<span class=\"token operator\">:</span> <span class=\"token punctuation\">[</span><span class=\"token operator\">...</span>value<span class=\"token punctuation\">]</span>\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function-variable function\">getValues</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">const</span> values <span class=\"token operator\">=</span> <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">.</span><span class=\"token function\">getValues</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n        console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span>values<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n    <span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n\n        <span class=\"token keyword\">return</span> <span class=\"token punctuation\">(</span>\n            <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Form</span></span> <span class=\"token attr-name\">field</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">FormItem</span></span> <span class=\"token attr-name\">required</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Upload</span></span>\n                        <span class=\"token attr-name\">listType</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>text<span class=\"token punctuation\">\"</span></span>\n                        <span class=\"token attr-name\">name</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>upload<span class=\"token punctuation\">\"</span></span>\n                        <span class=\"token attr-name\">action</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>https://www.easy-mock.com/mock/5b713974309d0d7d107a74a3/alifd/upload<span class=\"token punctuation\">\"</span></span>\n                        <span class=\"token attr-name\">defaultValue</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>value<span class=\"token punctuation\">}</span></span>\n                    <span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Upload</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Upload</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">FormItem</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span> <span class=\"token attr-name\">onClick</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>setValues<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>primary<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span>margin<span class=\"token operator\">:</span> <span class=\"token string\">'0 0 10px'</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Set Data</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">&amp;nbsp;&amp;nbsp;\n                    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span> <span class=\"token attr-name\">onClick</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>getValues<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>primary<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span>margin<span class=\"token operator\">:</span> <span class=\"token string\">'0 0 10px'</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Get Data</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">&amp;nbsp;&amp;nbsp;\n                    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span> <span class=\"token attr-name\">onClick</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">.</span><span class=\"token function\">reset</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>primary<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span>margin<span class=\"token operator\">:</span> <span class=\"token string\">'0 0 10px'</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Reset</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">&amp;nbsp;&amp;nbsp;\n                    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Button</span></span> <span class=\"token attr-name\">onClick</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>field<span class=\"token punctuation\">.</span><span class=\"token function\">validate</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>primary<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span>margin<span class=\"token operator\">:</span> <span class=\"token string\">'0 0 10px'</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Validate</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Button</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n                </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n            </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Form</span></span><span class=\"token punctuation\">></span></span>\n        <span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n<span class=\"token punctuation\">}</span>\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">App</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div>"}