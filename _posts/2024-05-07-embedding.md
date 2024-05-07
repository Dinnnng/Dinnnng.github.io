---
layout:     post
title:      MTEB排行榜上AI Embedding模型大盘点
subtitle:   优秀的Embedding模型大盘点
date:       2024-05-07
author:     Wade
header-img: img/WechatIMG98.jpg
catalog: true
tags:
    - RAG
    - 增强检索
    - embedding
---
大家好，今天我们来聊聊AI领域中一个非常核心的技术——embedding模型。在人工智能的世界里，embedding模型就像是给文本穿上了一件“数字化”的外衣，让机器能够更好地理解和处理语言。无论是搜索引擎、推荐系统还是自然语言处理的各种应用，embedding模型都扮演着至关重要的角色。下面，我将为大家整合目前市面上一些优秀的embedding模型，以及它们的相关信息和链接，希望能帮助到对这一领域感兴趣的朋友。

市面上优秀的embedding模型

[Massive Text Embedding Benchmark (MTEB) ](https://huggingface.co/spaces/mteb/leaderboard)2024-05-06

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=OTlkOWQ0OWIzYzllMDE3MjkxZDZmZjk2OTQyNjcxNDFfRGpIcVpvdHI5UXFZaTFPeDNuYUFpMjE1ZWhKeFJyZE9fVG9rZW46VHJuZWJRdHNCb3kxS094bTBPSmNtNW1obnhjXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 1. **Voyage**

Voyage团队认为业界对嵌入模型的重视程度远远不够，因此他们投入了5年时间，收集了海量的训练数据和预/后处理方法，打造出了SOTA的嵌入模型。Voyage的特点在于高检索精度，在HuggingFace提出的MTEB数据集上的评分超过了OpenAI，成为新的SOTA。Voyage的学术顾问团队也是星光熠熠，包括斯坦福人工智能实验室主任Christopher Manning和AI领域著名华人学者李飞飞等。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=MzcwNmQwZWE1MTAxMzU0N2Y3OWJlZjU2ZGU0Zjk3MmVfZGV6ZlJsS01yMFFuWXJhM2loUmtaSXo2TlRyamtiSndfVG9rZW46QnE1cGJVNmZEbzh2a0t4aGNTZGN5NjZGbk1iXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=NmQ2YzUyNjg3NzM4MWU0OTE3ZjgxZGRmZDAxYjhhNWZfU3E4eVFQZk1OR0xKUnpTdTBWU0gxY3ZjVzZCU2lEQ2RfVG9rZW46RGYxamJvNU5Kb1dzb0l4SlZXNWNJVXFybkpjXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 2. **Mistral**

微软最近发布的text embedding模型E5-mistral-7b-instruct在MTEB数据集上取得了优异的成绩。该模型利用LLM生成了接近100种语言的高质量且多样化的训练数据，并通过纯decoder的LLM在合成数据上进一步finetune。Mistral-7b-instruct展示了即使仅使用合成数据，也能训练出媲美主流SOTA模型的text embedding。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=ZjFlNTMyNjI4ZGZiNzU2OGFmZTg0ZGNhZGZhMTI2ODlfV3d6c1pyMHlCeTdXNWtibWY3SzVQdGNoYXI2MVZhaDJfVG9rZW46VGY0cWJNMXQwb09BUXF4Q1p1TGNXR25GbndlXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 3. **Qwen**

Qwen模型采用了GTE统一文本表示，基于预训练的文本表示模型，通过双塔结构（Dual Encoder）训练。在Dual Encoder框架中，Query和Document文本通过预训练语言模型编码后，通常采用预训练语言模型[CLS]位置的向量作为最终的文本向量表示。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=ZjE2ZGZmODNlNDFmYzI2MWZkZjkzNjhmMzFjMGE5YjZfV09Vb3BLWTNmQjc1RWdIR01iUklnTFpPanNrejQ2bHJfVG9rZW46TGQ2YWJJbDBub3FaWHV4V3VEeGM0TUIwbjdnXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=NzcwYjQ1MTEwNzRlODQ1NDIwNzgxMWRjMjZkMDI0MTFfZXRTdElhQmk1VDl0Q2ZMOGkzM1EyZkhmRGlzM0FSSnJfVG9rZW46TllySGJiT3dab3RzczR4Y05lTWM3Q2lmbmFjXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=OWU4ZDg5NjY5ODUyYWJhZjk2YmFmNmYwMDdlMTU4YmJfbXJPRVp5Sk1mdmVVMHNCbXVSNE9WOUlvcTMxSUJaRkNfVG9rZW46WGRXSGJyNElvb1lhWER4cll6QWNKSVZzbmhmXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=YWQzNzBiYWRmMjc4YzFkMDJhZjgyMzc2YjBhYjU3MTdfeVJZR1E3WkhJMzhkQjRYQlc3dTJObmxSWWdpWkpBeEZfVG9rZW46UVBIQ2I0V3lmb2xLWkd4N05aNWNRY0N6bjVnXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=ODVmYjIwYmFlY2I5NzMwMzFlN2JmMjI5OGNiMjc3MDNfODRzWllxdW5ad0l6VU1MR0NnQjY5VkFObEpUdk41bkZfVG9rZW46SURTYWJjYUFKb1o0Yzd4WXlPSGNnWXVvbnhkXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 4. **BGE-M3**

智源发布的BGE-M3模型支持超过100种语言，具备领先的多语言、跨语言检索能力。BGE-M3模型一站式集成了稠密检索、稀疏检索、多向量检索三种检索功能，在多个评测基准中达到最优水平。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=ZjY4YjhiNWJlNTc4OTZhZjAyODY5YmM1M2JkZGU4ZDdfNXpqRlU1VnVJUWhNNGl6Q3BvZVd6MDk0NklMZ2hGdFFfVG9rZW46T3Y5cGJ0M0RGbzNnbjV4THdyRmNRRXZ2blExXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 5. **BCEmbedding**

网易有道开源的BCEmbedding模型，具备中英双语和跨语种能力，覆盖多领域，设计了标签分配方法，使得Embedding模型可以尽可能召回，而Reranker模型则负责精排和低质量过滤。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=Njk3MmM5MDMyNDBkMThiYWRiZWI0ZmNkMjg5MTY1MDJfMTJ5MDhGaXNrWkRlYnBXTFlUbElBaThta2VGUlZHcTRfVG9rZW46VDcyR2J2M0Zzb0pXOVZ4aXpaUGNhNllqbkp0XzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 6. **Cohere**

Cohere提供了闭源的embedding服务，通过API收费的方式提供服务。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=N2M2ODQ5MmY5YjUyMzg0NzVhYWUyMzk3MGIwMTllZDVfOUd4WFVjdkhSbDJBV2JHVTY1ck5wUzk1SWtpZlcyQTJfVG9rZW46VnlEY2JkalEyb0lrTnd4T0JyZ2NoamRrbjdnXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 7. **Jina**

Jina.ai提供的embedding服务也是闭源的，同样通过API收费。

![img](https://qn5ocuvtnb.feishu.cn/space/api/box/stream/download/asynccode/?code=YTJkOTk1YmExYmE3ZTdlYzY1ZmU0YjRmOWVkZDE0YzdfcmtvNVBsZUxURXFybmcwT3I3WEx3VGZuU002ZEcwNkFfVG9rZW46UVBBQmJWQmlyb2FoMmR4UVlFNmNBcW9jbktnXzE3MTUwODk3Mjg6MTcxNTA5MzMyOF9WNA)

### 8. **GritLM-7B**

GritLM是一种生成表示指令调整语言模型，它将文本表示（嵌入）和文本生成统一到一个模型中，在这两类任务中都取得了最先进的性能。

以上便是目前市面上一些较为优秀的embedding模型的概览。每个模型都有其独特的优势和应用场景，无论是学术研究还是商业应用，它们都提供了强大的支持。如果你对这些模型感兴趣，可以通过提供的链接进一步了解它们的详细信息和使用方式。记住，embedding模型是RAG（Retrieval-Augmented Generation）技术的核心，对于希望深入AI领域的你来说，了解这些模型将大有裨益。