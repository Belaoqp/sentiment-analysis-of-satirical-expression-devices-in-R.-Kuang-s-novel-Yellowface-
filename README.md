- Файл "ПРОМПТ" содержит промпт для ИИ, который был использован для данного исследования.\
На 17 строке вставлялся текст в фигурных скобках {{ текст }}.

- Файл Сентимент-анализ.pdf представляет собой сентимент-анализ, в котором содержится:\
&ensp;1.69 контекстов, использовавшихся для анализа с пометкой типов языковых средств под таблицей.\
&ensp;2.Автоматический сентимент-анализ, выполненный с помощью ИИ и вышеописанного промпта.\
&ensp;3.Ручной сентимент-анализ, выполненный непосредственно каждым участником.\
&ensp;4.Диаграмма, сравнивающая сентимент-анализ ИИ и ручной анализ.\
&ensp;5.Легенда по обозначению цветов языковых средств в самом низу.

> [!NOTE]
> Для автоматического сентимент-анализа материала был создан промпт, основанный на технике Chain-of-Thought[^1], однако были также рассмотрены варианты Zero-shot и Few-shot Prompting[^2], где ИИ даётся одна задача и несколько готовых примеров (либо один в технике Zero-shot), после чего ИИ даёт ответ, опираясь на пример(ы). При этом мы остановились на Chain-of-Thought, т.к. в таком случае ИИ даётся конкретная инструкция о его последующих действиях, благодаря чему он действует в строго заданных рамках, и шанс выдать неуместный ответ минимизируется. Для реализации автоматического сентимент-анализа был использован DeepSeek версии DeepSeek-V4-Pro (Expert) с включённой функцией «Search». Выбор DeepSeek в качестве ИИ обусловлен отсутствием лимита использования и низким процентом ошибок в ответах в сравнении с другими ИИ, где Claude находится на 1-м месте, а DeepSeek – на 2-ом[^3].



[^1]: 1. Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed Chi, Quoc Le, Denny Zhou. Chain-of-Thought Prompting Elicits Reasoning in Large Language Models (v6) // NIPS'22: Proceedings of the 36th International Conference on Neural Information Processing Systems. 2023. URL: https://arxiv.org/abs/2201.11903 (дата обращения: 10.04.2026).
[^2]: 2. Laria Reynolds, Kyle McDonell. Prompt Programming for Large Language Models: Beyond the Few-Shot Paradigm // CHI EA '21: Extended Abstracts of the 2021 CHI Conference on Human Factors in Computing Systems. 2022. URL: https://dl.acm.org/doi/10.1145/3411763.3451760 (дата обращения: 10.04.2026).
[^3]: 3. Tianchen Gao, Jiashun Jin, Zheng Tracy Ke, Gabriel Moryoussef. Comparison of DeepSeek and other LLMs // The American Statistician. 2026. URL: https://www.tandfonline.com/doi/full/10.1080/00031305.2025.2611010 (дата обращения: 18.04.2026).
