# Pedro Henrique

### Engenharia de software aplicada à inteligência artificial

Construo projetos que conectam modelos de IA a aplicações reais, com atenção a
integração, execução, testes e avaliação. Meu foco é **AI Engineering**: transformar
modelos e dados em sistemas que possam ser executados, inspecionados e melhorados.

Minha experiência apresentada aqui reúne **pesquisa PIBIC com áudio** e um
**projeto colaborativo DevTitans de IA generativa no Android**.

[GitHub](https://github.com/pedrobelota) · [Hugging Face](https://huggingface.co/phbg) · [Datasets e referências de modelos](https://huggingface.co/collections/phbg/devtitans-and-pibic-ai-engineering-6ae553217b5be2d991b7e904)

## Projetos em destaque

### 01 · Smart Notifications — LLM no próprio Android

**Transformar rajadas de notificações em resumos curtos em português, com inferência local.**

No projeto colaborativo DevTitans, minha frente é a integração de LLM. A PoC usa
Gemma e LiteRT-LM, com engenharia de prompt, streaming de tokens, controle de contexto
e gestão do engine nativo. O fluxo agrupa notificações e publica um resumo no Android.

- **Engenharia:** Kotlin, inferência on-device, debounce, prevenção de loop, testes JVM e CI com build do APK.
- **Dados:** 3.707 exemplos sintéticos publicados no Hugging Face, com splits e auditoria.
- **Estado:** PoC com validação de bancada relatada. Piloto QLoRA preparado; treinamento e resultados ainda pendentes. O piloto Gemma 3 1B é separado do modelo usado no Android.

[Código e arquitetura](https://github.com/pedrobelota/android-smart-notifications) · [Contribuições e evidências](https://github.com/pedrobelota/android-smart-notifications/blob/feat/poc-litert-gemma/docs/EVIDENCE.md) · [Dataset](https://huggingface.co/datasets/phbg/smart-notifications-synthetic) · [Experimento QLoRA](https://github.com/pedrobelota/android-smart-notifications/tree/feat/poc-litert-gemma/notebooks)

### 02 · Coach Emotion Analysis — pesquisa e pipeline de áudio

**Transformar áudio ou vídeo em hipóteses de emoção alinhadas no tempo e avaliar os resultados.**

Projeto PIBIC que integra transcrição Whisper, classificação acústica Wav2Vec2 e
regras do domínio de futebol. O trabalho inclui processamento temporal, fusão de
evidências, avaliação com baselines, CLI e uma demonstração local com API de áudio.

- **Engenharia:** Python, PyTorch, Transformers, FastAPI, Docker e CI em Linux/Windows.
- **Pesquisa:** métricas por classe, análise de desbalanceamento e separação entre execução funcional e qualidade preditiva.
- **Estado:** pipeline funcional; o estudo piloto apresenta limitações de classificação. Corpus privado; apenas exemplos sintéticos de formato são públicos.

[Código e execução](https://github.com/pedrobelota/coach-emotion-analysis) · [Método](https://github.com/pedrobelota/coach-emotion-analysis/blob/main/docs/methodology.md) · [Resultados e limitações](https://github.com/pedrobelota/coach-emotion-analysis/blob/main/docs/results.md) · [Exemplos de dados](https://huggingface.co/datasets/phbg/coach-emotion-synthetic-schema)

## Competências demonstradas no código

| Área | Evidência |
| --- | --- |
| Integração de modelos | LLM com runtime nativo Android; ASR e classificação acústica em Python |
| Dados e avaliação | Dados sintéticos auditados, alinhamento temporal, métricas por classe e baselines |
| Entrega de software | CLI, API, Docker, testes automatizados e GitHub Actions |
| Experimentação com LLMs | Engenharia de prompt e protocolo de adaptação QLoRA em andamento |

## Como apresento meu trabalho

Cada projeto explicita autoria, modelos de terceiros, evidências de execução e
limitações. O histórico colaborativo é preservado. Assistentes de IA apoiaram revisão,
documentação e manutenção; a responsabilidade por compreender e validar o trabalho
continua sendo minha. Resultados de treinamento só são apresentados após execução e avaliação.

---

**English:** AI Engineering portfolio with on-device LLM integration for Android and
a research audio pipeline. Each repository includes technical documentation,
reproducibility instructions, attribution and evaluation limitations.
