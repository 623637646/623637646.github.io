---

layout: post
title: "IOS UI Github开源代码"
description: "github里，收集的IOS UI开源代码"
category: IOS
tags: [IOS,Github,UI,开源]
source_github_items: [
     {
          source_keywords: [菊花,进度条,加载,等待],
          source_projects: [
                         {
                              source_url: "https://github.com/jdg/MBProgressHUD",
                              source_description: "常用",
                              source_imgs: [
                              "https://camo.githubusercontent.com/8211f8a4fa848499e174fa3d6125adb2044c182e/687474703a2f2f646c2e64726f70626f782e636f6d2f752f3337383732392f4d4250726f67726573734855442f312d7468756d622e706e67",
                              ]
                         },

                         {
                              source_url: "https://github.com/mrackwitz/MRProgress",
                              source_imgs: [
                                        "https://github.com/mrackwitz/MRProgress/raw/master/Images/screenshot_004_2.jpg",
                                        "https://github.com/mrackwitz/MRProgress/raw/master/Images/circular_indeterminate.gif",
                              ]
                         },
                         
                         {
                              source_url: "https://github.com/TransitApp/SVProgressHUD",
                              source_imgs: [
                                        "https://camo.githubusercontent.com/6ed028acbf67707d622344e0ef1bc3b098425b50/687474703a2f2f662e636c2e6c792f6974656d732f32473146315a304d306b306832553356317033392f535650726f67726573734855442e676966",
                              ]
                         },
                         {
                              source_url: "https://github.com/Marxon13/M13ProgressSuite",
                              source_imgs: [
                                        "https://camo.githubusercontent.com/09f2c629a458564176f6096db0be1a69b8eaad92/68747470733a2f2f7261772e6769746875622e636f6d2f4d6172786f6e31332f4d313350726f677265737353756974652f6d61737465722f526561646d655265736f75726365732f55494e617669676174696f6e4261722e676966",
                                        "https://camo.githubusercontent.com/43c88763dfb22758f0f291404655e93d346b0b7d/68747470733a2f2f7261772e6769746875622e636f6d2f4d6172786f6e31332f4d313350726f677265737353756974652f6d61737465722f526561646d655265736f75726365732f4261722e676966",
                                        "https://camo.githubusercontent.com/e54ca5075db0dfafc39bdce255f0432bd925343c/68747470733a2f2f7261772e6769746875622e636f6d2f4d6172786f6e31332f4d313350726f677265737353756974652f6d61737465722f526561646d655265736f75726365732f52696e672e676966",
                              ]
                         },

          ]
     },
     {
          source_keywords: [侧边栏,抽屉],
          source_projects: [
                         {
                              source_url: "https://github.com/romaonthego/RESideMenu",
                              source_imgs: [
                                        "https://raw.githubusercontent.com/romaonthego/RESideMenu/master/Demo.gif?2",
                              ]
                         },

                         {
                              source_url: "https://github.com/erichoracek/MSDynamicsDrawerViewController",
                              source_imgs: [
                                        "https://camo.githubusercontent.com/dd10d9cce48a326b7124daa8e6e6ff8c8b552505/68747470733a2f2f7261772e6769746875622e636f6d2f6d6f6e6f7370616365636f6c6c6563746976652f4d5344796e616d69637344726177657256696577436f6e74726f6c6c65722f6d61737465722f53637265656e73686f74732f666c696e672e676966",
                              ]
                         },
                         
                         {
                              source_url: "https://github.com/mutualmobile/MMDrawerController",
                              source_imgs: [
                                        "https://camo.githubusercontent.com/171bc22d1f4ad13f7be22cf546c2644176066193/687474703a2f2f6d757475616c6d6f62696c652e6769746875622e696f2f4d4d447261776572436f6e74726f6c6c65722f4578616d706c65496d616765732f6578616d706c65312e706e67",
                              ]
                         },
                         
                         {
                              source_url: "https://github.com/pkluz/PKRevealController",
                              source_imgs: [
                                        "https://camo.githubusercontent.com/0fb9edaace4d7ccbf34aeeae691dff0b3423fe03/687474703a2f2f696d6733342e696d616765736861636b2e75732f696d6733342f313435362f686e73312e706e67",
                              ]
                         },
                         
                         {
                              source_url: "https://github.com/romaonthego/REFrostedViewController",
                              source_imgs: [
                                        "https://github.com/romaonthego/REFrostedViewController/raw/master/Demo.gif",
                              ]
                         },
                         
                         {
                              source_url: "https://github.com/JVillella/JVFloatingDrawer",
                              source_imgs: [
                                        "https://camo.githubusercontent.com/44098d6ff4f858b06190b4d39afac8f51d4c7803/687474703a2f2f6a76696c6c656c6c612e6769746875622e696f2f4a56466c6f6174696e674472617765722f53637265656e73686f74732f616e696d617465642d6472617765722d6f70656e2d706f7274726169742e676966",
                              ]
                         },
          ]
     },
]

---

<head>
    <link rel="stylesheet" href="//cdn.bootcss.com/bootstrap/3.3.5/css/bootstrap.min.css">
    <script src="//cdn.bootcss.com/jquery/1.11.3/jquery.min.js"></script>
    <script src="//cdn.bootcss.com/bootstrap/3.3.5/js/bootstrap.min.js"></script>
    <style type="text/css">
	.css_project_img_div {
		height:150px;
	}
    .css_project_img{
        max-height:100%;
        max-width:33%;
    }
    </style>
</head>


<div>
	
	{% for github_item in page.source_github_items %}
		<h3>
			{% for keyword in github_item.source_keywords %}
				{{ keyword }}
				{% if forloop.rindex != 1 %}
					,
				{% endif %}
			{% endfor %}    
		</h3>
		{% for project in github_item.source_projects %}
			<div class="css_project_img_div">
				{% for img in project.source_imgs %}
					<img class="css_project_img img-rounded" src="{{img}}" alt="效果图">
				{% endfor %}			
			</div>
			<h4>
                <a href="{{project.source_url}}" class="btn btn-default" role="button">{{project.source_url | split:'/' | last}}</a>
                <small>{{project.source_description}}</small>
			</h4>
		{% endfor %}
	{% endfor %}
	
</div>