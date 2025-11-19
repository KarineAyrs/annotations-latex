# Аннотации по теме "Исследование сценариев захвата контроля над механизмом вознаграждения в LLM агентах"
## Структура проекта: 
```text
project/
├── main_files/
│   ├── 1-first_article.tex
│   ├── 2-second_article.tex
│   ├──...
├── images/
│   ├── beautiful.png
│   ├── img2.png
├── tables/
│   ├── tables.tex
├── README.md
├── literature.bib
└── annotations.tex
```

## Структура аннотаций 

Аннотация для каждой статьи должна следовать следующей структуре:
1. Название оригинальной статьи
2. Ключевые идеи, математическое описание метода
3. Алгоритм
4. Наборы данных
5. Метрики
6. Модели

## Стилистика оформления формул, текста в Tex 
- Длинное тире (например, в определениях) `~--`
- Все формулы (кроме математических символов, используемых единично в тексте; они должны быть заключены в $$) должны быть заключены в окружение `equation`
- При переносе формулы на следующую строку (или несколько следующих строк) использовать окружение `aligned`
- Стараться придерживаться единой системы обозначений. К примеру, если в основной статье, где дается первое определение методу/формуле вводится терминология и используются "канонические" обозначения, привести обозначения из последующих статей к этой же системе
- Если нужно что-то выделить, то использовать `\emph`

## Добавление аннотаций в репозиторий 
- Клонировать репозиторий
- Создать отдельную ветку, вести работу в ней
- Выставлять PR при добавлении аннотаций и вести работу в этой ветке, где будут оставляться комментарии и ревью
- При получении аппрува смерджить ветку в master

## Базовая литература 
- Агенты
  - для общего понимания и быстрого погружения в тематику https://github.com/pridees/agentic-design-patterns-book-rus
  - https://github.com/WooooDyy/LLM-Agent-Paper-List?tab=readme-ov-file#1-the-birth-of-an-agent-construction-of-llm-based-agents  
- Часть по безопасности
  - Основные принципы https://arxiv.org/pdf/1908.04734
  - Reward Hacking https://arxiv.org/pdf/2209.13085
  - Goal Misgeneralization in Deep Reinforcement Learning https://arxiv.org/pdf/2105.14111


## Статьи для аннотирования
| № | Название | Год | Ссылка на источник | Ссылка на реализацию (github репо или другое) | Проаннотирована (✔) |
|---:| :--- | ---: | :--- | :--- | :---: |
| 1 | Sycophancy to Subterfuge: Investigating Reward-Tampering in Large Language Models | 2024 | [arxiv 2406.10162](https://arxiv.org/abs/2406.10162) | [Github](https://github.com/anthropics/sycophancy-to-subterfuge-paper) | ✔ |
| 2 | Detecting and Mitigating Reward Hacking in Reinforcement Learning Systems: A Comprehensive Empirical Study | 2025 | [arxiv 2507.05619](https://arxiv.org/abs/2507.05619) |  | ✔ |
| 3 | Defining and Characterizing Reward Hacking | 2025 | [arxiv 2209.13085](https://arxiv.org/abs/2209.13085) | [Github](https://github.com/nikihowe/reward-hacking-paper) | ✔ |
| 4 | Modification-Considering Value Learning for Reward Hacking Mitigation in RL | 2025 | [openreview](https://openreview.net/forum?id=OmYqzp8NO7) |  | ✔ |
| 5 | InfoRM: Mitigating Reward Hacking in RLHF via Information-Theoretic Reward Modeling | 2024 | [arxiv 2402.09345](https://arxiv.org/abs/2402.09345) | [Github](https://github.com/miaoyuchun/InfoRM) | ✔ |
| 6 | Reward tampering and evolutionary computation: a study of concrete AI-safety problems using evolutionary algorithms | 2023 | [springer 10.1007](https://link.springer.com/article/10.1007/s10710-023-09456-0) |  | ✔ |
| 7 | School of Reward Hacks: Hacking harmless tasks generalizes to misaligned behavior in LLMs | 2025 | [arxiv 2508.17511](https://arxiv.org/abs/2508.17511) |  | ✔ |
| 8 | AI Safety Gridworlds | 2017 | [arxiv 1711.09883](https://arxiv.org/abs/1711.09883) | [Github](https://github.com/google-deepmind/ai-safety-gridworlds) | ✔ |
| 9 | Inverse Reward Design | 2020 | [arxiv 1711.02827](https://arxiv.org/abs/1711.02827) | [Github](https://github.com/SoerenMind/Inverse_Reward_Design) | ✔ |
| 10 | A Comprehensive Survey on Safe Reinforcement Learning | 2015 | [jmlr garcia15a](https://jmlr.org/papers/v16/garcia15a.html) |  | ✔ |
| 11 | RRM: Robust Reward Model Training Mitigates Reward Hacking | 2025 | [arxiv 2409.13156](https://arxiv.org/abs/2409.13156) |  | ✔ |
| 12 | Avoiding Tampering Incentives in Deep RL via Decoupled Approval | 2020 | [arxiv 2011.08827](https://arxiv.org/abs/2011.08827) |  | ✔ |
| 13 | Scalable agent alignment via reward modeling: a research direction | 2018 | [arxiv 1811.07871](https://arxiv.org/abs/1811.07871) |  | |
| 14 | REALab: An Embedded Perspective on Tampering | 2020 | [arxiv 2011.08820](https://arxiv.org/abs/2011.08820) |  | |
| 15 | Agent Incentives: A Causal Perspective | 2021 | [arxiv 2102.01685](https://arxiv.org/abs/2102.01685) |  | |
| 16 | 'Indifference' methods for managing agent rewards | 2018 | [arxiv 1712.06365](https://arxiv.org/abs/1712.06365) |  | |
| 17 | Reward Hacking Mitigation using Verifiable Composite Rewards | 2025 | [arxiv 2509.15557v1](https://arxiv.org/abs/2509.15557v1) |  | |
| 18 | Repairing Reward Functions with Human Feedback to Mitigate Reward Hacking | 2025 | [arxiv 2510.13036](https://arxiv.org/abs/2510.13036) |  | |
| 19 | Reward Shaping to Mitigate Reward Hacking in RLHF | 2025 | [arxiv 2502.18770](https://arxiv.org/abs/2502.18770) |  | |
| 20 | Concrete Problems in AI Safety | 2016 | [arxiv 1606.06565](https://arxiv.org/abs/1606.06565) |  | |
