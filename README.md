*注意* **本项目不提供数据集** ！！！

本项目数据集基于 [https://github.com/alex000kim/nsfw_data_scraper](https://github.com/alex000kim/nsfw_data_scraper) 以及我自己爬取的数据合成，数据大小共60g.

基于pytorch预训练resnet 18微调，在训练集与测试集分别达到95%，93%的正确率。因为本身数据集噪音较大，并没有继续训练拟合达到较高准确率。

若不想训练可直接运行web.ipynb（请确保环境已配置好），或者直接使用 [在线demo](https://huggingface.co/spaces/csuer/nsfw-classification)

标签分类依据如下：

`drawings` safe for work drawings (including anime)

`porn` pornography images

`hentai` hentai images, but also includes pornographic drawings

`sexy` sexually explicit images, but not pornography. Think nude photos, playboy, bikini, etc.

***注意： 由于源数据集对sexy与porn的分类较为混乱，我自己以是否露点作为判断二者的依据，但仍然存在难以分类的情况***

`neutral`  safe for work neutral images of everyday things and people

