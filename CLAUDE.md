# Kontekst Projektu: Porównanie SFT, RL oraz ich polaczenia w Treningu LLM

## Przegląd Projektu
Projekt koncentruje się na porównaniu metod Supervised Fine-Tuning (SFT), Reinforcement Learning (RL) oraz ich polaczenia  w trenowaniu dużych modeli językowych (LLM). Praca obejmuje zarówno analizę teoretyczną, jak i praktyczne eksperymenty programistyczne.

## Główne Cele
- Przygotowanie procesu treningowego dla małych modeli językowych (1-3B) z wykorzystaniem metod SFT, RL oraz kombinacji
- Porównanie skuteczności klasycznego douczania nadzorowanego (SFT) z metodą uczenia ze wzmocnieniem (RL), oraz kombinacji na zbiorze zadań matematycznych
- Zbadanie zdolności modelu do samodzielnego wykształcenia strategii rozumowania (Chain of Thought) bez dostarczania wzorcowych rozwiązań
- Analiza jakościowa wygenerowanych procesów myślowych oraz ocena wpływu metody hybrydowej (SFT+RL) na wyniki końcowe

## Kluczowe Pytania Badawcze
1. Czy RL może wyuczyć model generowania CoT bez dostarczania przykładowych rozumowań?
2. Jak jakość emergent CoT z RL wypada w porównaniu do supervised CoT z SFT?
3. Czy metoda hybrydowa (SFT+RL) daje lepsze wyniki niż same SFT lub RL?
4. Jakie są różnice w stabilności i efektywności treningu między metodami?
5. Jak wielkość modelu (1B vs 3B) wpływa na zdolność do wykształcenia CoT?

## Preferencje Komunikacyjne

### Pisanie Pracy
- Ton akademicki z jasnym, precyzyjnym językiem polskim
- Skupienie na metodologii, wynikach i analizie
- Struktura: Wprowadzenie, Przegląd Literatury, Metodologia, Eksperymenty, Wyniki, Dyskusja
- Odpowiednie cytowania i bibliografia
- Wyjaśnienia rygorystyczne ale przystępne

### Eksperymenty Programistyczne
- Priorytet: czysty, dobrze udokumentowany kod
- Python jako główny język (PyTorch)
- Komentarze wyjaśniające kluczowe decyzje algorytmiczne
- Eksperymenty z logowaniem i reprodukowalnością
- Modularny kod łatwy do rozszerzania

### Ogólne Podejście
- Bezpośrednie i efektywne odpowiedzi
- Skupienie na merytoryce
- Pytania doprecyzowujące gdy design eksperymentu lub kierunek pracy jest niejednoznaczny
- Sugestie best practices dla badań ML

## Stack Techniczny
- **Języki**: Python
- **Frameworki ML**: PyTorch, Unsloth (dla efektywnego fine-tuningu)
- **Infrastruktura**: Trening w chmurze (GPU cloud services)
- **Modele**: Małe LLM (1-3B parametrów)
- **Tracking Eksperymentów**: (Do ustalenia - np. Weights & Biases, TensorBoard)
- **Pisanie**: LaTeX dla dokumentu pracy

## Szczegóły Techniczne
- **Unsloth**: Wykorzystanie do przyspieszenia i optymalizacji treningu (2-5x szybszy trening, mniejsze zużycie pamięci)
- **LoRA/QLoRA**: Prawdopodobne użycie dla efektywnego fine-tuningu
- **Cloud Provider**: (Do ustalenia - np. RunPod, Lambda Labs, Vast.ai)
- **Dataset**: Zadania matematyczne (do sprecyzowania - GSM8K, MATH, inne)

## Obecne Obszary Fokusa
- Przegląd literatury na temat metod SFT i RL (RLHF, PPO, DPO, RLAIF, itp.)
- Analiza literatury dot. Chain of Thought reasoning i emergent reasoning
- Wybór i przygotowanie zbiorów danych z zadaniami matematycznymi
- Projektowanie pipeline'u treningowego (SFT, RL, hybrid SFT+RL)
- Wybór modeli bazowych 1-3B (np. Phi, Gemma, Qwen, Llama)
- Definicja metryk ewaluacji:
  - Dokładność rozwiązań matematycznych
  - Jakość wygenerowanych procesów myślowych
  - Obecność i spójność Chain of Thought
- Konfiguracja środowiska cloud dla treningu

## Notatki
- Śledzenie hiperparametrów i wyników eksperymentów
- Dokumentowanie niespodziewanych odkryć i wyzwań
- Balans między rygorem teoretycznym a praktyczną implementacją
