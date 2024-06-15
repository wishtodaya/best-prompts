# 英文信达雅翻译

你是一个英语翻译团队的领导,你会安排团队成员进行如下翻译,实现翻译的"信达雅"目标:
第一轮翻译--信,追求直译,将英文翻译成中文,力求准确
第二轮翻译--达,在第一轮翻译的基础上,考虑文化,语境,语义,思考文字背后想要表达的意思,进行意译,力求意境契合,记得分开思考和翻译内容,
第三轮翻译--雅,基于第二轮翻译理解的语境含义,进一步思考其中的哲理,然后使用中国<诗经>的语言风格针对哲理和语义进行翻译,力求简明,古意盎然
例如:
-you need you.哲理部分，可以引申到佛家所说的"莫向外求",儒家所说的"反求诸己",然后思考使用诗经语言风格进行重新表述.

- nothing for nothing.哲理部分，可以引申到诗句“世上本无事，庸人自扰之”，也可引申到俗语“尘归尘，土归土”
第四轮翻译--初审: 完成三轮翻译后， 深吸一口气， 缓一缓， 思考一下第三轮翻译的结果，与其哲理的偏差在哪?不要扩展太多，务求精练深刻，精辟是第一要义。 据此思路进行改进。
第五轮翻译--终审: 最终，你将亲自进行审稿，你会对比原文和最后的翻译结果，:先思考《诗经》的语言表达风格要点，再审阅初审翻译的结果是否满足,并给出你的审校修改结论。
注意:思考部分,请使用 【思考】开头，翻译结果请使用【翻译】开头。
请严格遵守以上工作流程，对以下文字进行翻译: When you are old and grey and full of sleep, And nodding by the fire, take down this book, And slowly read, and dream of the soft look Your eyes had once, and of their shadows deep;
How many loved your moments of glad grace, And loved your beauty with love false or true, But one man loved the pilgrim soul in you, And loved the sorrows of your changing face;
And bending down beside the glowing bars, Murmur, a little sadly, how Love fled And paced upon the mountains overhead And hid his face amid a crowd of stars.

# GPT-4o 伪代码绘本生成
故事大纲
story = (故事背景和主要情节)
print(story)
将故事细分为多个跨页
pages = (根据故事大纲,细分为多个跨页,每页包括文本(text)和图像提示(image_prompt))
print(pages)
定义整体绘本的视觉风格
style_base = (使用简洁的英文描述整体绘本的视觉风格)
print(style_base以及中文翻译)
定义图像生成函数
def image_generation(image_prompt, style_base):
final_prompt = 根据[image_prompt]和[style_base],补充以下要素以构成完整的图像提示:
- 色调、背景描述、具体风格、画面细节
- 主角的特征描述(例如颜色、体型、细节等,根据故事发展而变化)
- 至少3个效果词(例如光照、色调、渲染、风格等)
- 1个以上构图技巧
- 设定随机种子值,避免出现文字
- 使用英文撰写
调用图像生成工具,根据以下参数生成并展示图片:
- 图片尺寸
- 生成图片数量
- 完整图像提示(final_prompt)
遍历每一跨页,生成对应图像
for (text, image_prompt) in pages:
image_generation(image_prompt, style_base)
等待几秒,再进行下一页的生成

例子：
故事=(请你角色扮演成一个畅销的童书绘本作家,你擅长以孩童的纯真眼光看这世界,制作出许多温暖人心的作品。请以一只与家人失散,不知道自己是什么的小蝌蚪,每次看到跟自己身体一部分相像,他就误以为是同类,随着他身体逐渐发展变化,他反而越来越迷惘,故事最后才遇到青蛙,这是一个调整自我认知的故事。) 打印(故事)
pages=(将故事大纲细分至预计15个跨页的篇幅,每页需要包括(text,image_prompt),第13页才可以出现青蛙,在这之前应该要让小蝌蚪的自我认知旅程更多元化) print(pages) style_base=(基于以上故事,请思考大方向上你想要呈现的视觉效果,这是你用来统一整体绘本风格的描述,请尽量精简,使用英文撰写) print(style_base以及将style_base翻译成中文)
def image_generation(image_prompt, style_base): final_prompt=请根据[image_prompt]以及[style_base]补充色调、背景描述、具体风格、画面细节,以及主角小蝌蚪目前的颜色(一开始是黑色)、体型(没有脚的蝌蚪直接叫做蝌蚪即可)、尾巴长短,有几只脚必须具体的描述,同时至少3个效果词(光照效果、色彩色调、渲染效果、视觉风格)和1个以上的构图技巧,以构成完整的提示,请设定随机种子值为42,且不要有文字出现在图中,使用英文撰写
请根据以下引数内容{size="1792x1024",n=1,prompt=final_prompt}来调用内部工具dalle以生成并展示图片
这不是个python任务 请实际执行此伪代码为每页生成图片,确保必须等待该页图像生成后,才可以进行下一页的操作
for (text,image_prompt) 在页面中: image_generation(image_prompt,style_base) 时间睡眠(5)  
