
# Árboles sintácticos en Mermaid

Este repositorio contiene un trabajo práctico de gramáticas en Prolog y su representación visual mediante **árboles de derivación** usando **Mermaid**.  
El objetivo es mostrar cómo se analizan oraciones en español, dividiéndolas en **sintagma nominal (SN)** y **sintagma verbal (SV)**, y representarlas gráficamente para facilitar la comprensión.

---

## Oración 1: Los aztecas hablan náhuatl
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: Los]
    SN --> N[N: aztecas]
    SV --> V[Verbo: hablan]
    SV --> N2[N: náhuatl]
```

## Oración 2: La dominación islámica disminuyó progresivamente
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: La]
    SN --> N[N: dominación islámica]
    SV --> V[Verbo: disminuyó]
    SV --> ADV[Adv: progresivamente]
```

## Oración 3: Los reyes católicos conquistaron Granada
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: Los]
    SN --> N[N: reyes católicos]
    SV --> V[Verbo: conquistaron]
    SV --> N2[N: Granada]
```

## Oración 4: El catalán es una lengua romance
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: El]
    SN --> N[N: catalán]
    SV --> V[Verbo: es]
    SV --> SN2[Sintagma Nominal]
    SN2 --> DET2[Det: una]
    SN2 --> N2[N: lengua romance]
```

## Oración 5: Los mayas resistieron la colonización española
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: Los]
    SN --> N[N: mayas]
    SV --> V[Verbo: resistieron]
    SV --> SN2[Sintagma Nominal]
    SN2 --> DET2[Det: la]
    SN2 --> N2[N: colonización española]
```

## Oración 6: Los sacerdotes evangelizaban a los indígenas
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: Los]
    SN --> N[N: sacerdotes]
    SV --> V[Verbo: evangelizaban]
    SV --> PP[Prep: a]
    PP --> SN2[Sintagma Nominal]
    SN2 --> DET2[Det: los]
    SN2 --> N2[N: indígenas]
```

## Oración 7: Las lenguas minoritarias de España han entrado en una nueva etapa
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: Las]
    SN --> N[N: lenguas minoritarias de España]
    SV --> V[Verbo: han entrado]
    SV --> PP[Prep: en]
    PP --> SN2[Sintagma Nominal]
    SN2 --> DET2[Det: una]
    SN2 --> N2[N: nueva etapa]
```

## Oración 8: El español es lengua oficial en diecinueve países de Latinoamérica
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: El]
    SN --> N[N: español]
    SV --> V[Verbo: es]
    SV --> N2[N: lengua oficial]
    SV --> PP[Prep: en]
    PP --> N3[N: diecinueve países de Latinoamérica]
```

## Oración 9: El terreno de Paraguay representaba desafíos de envergadura para los españoles
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: El]
    SN --> N[N: terreno de Paraguay]
    SV --> V[Verbo: representaba]
    SV --> N2[N: desafíos de envergadura]
    SV --> PP[Prep: para]
    PP --> SN2[Sintagma Nominal]
    SN2 --> DET2[Det: los]
    SN2 --> N3[N: españoles]
```

## Oración 10: Los niños monolingües de desarrollo normal pasan por varias etapas
```mermaid
graph TD
    O[Oración] --> SN[Sintagma Nominal]
    O --> SV[Sintagma Verbal]
    SN --> DET[Det: Los]
    SN --> N[N: niños monolingües de desarrollo normal]
    SV --> V[Verbo: pasan]
    SV --> PP[Prep: por]
    PP --> N2[N: varias etapas]
```



