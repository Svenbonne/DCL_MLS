# A Demo GitHub Repository for a Causal Case Study <a href="https://digitalcausalitylab.github.io/"><img src="figures/logo.png" align="right" width = "120" /></a>

This repository is created for demonstration purposes. Version control with Git and GitHub is taught in the [Digital Causality Lab](https://digitalcausalitylab.github.io/).

## First steps in GitHub

Participants of the [Digital Causality Lab](https://digitalcausalitylab.github.io/) should use this repo as a template and do the following steps.

1. Create your own GitHub repository.
  * You can either navigate to your GitHub profile, go to the repositories tab and click on **new**, or, 
  * You can use this template by clicking on the **Use this template** button.
![](figures/use_template_button.png)
2. Open an issues with a task. For example, the title could be "*Add some content to the `README.md` file*".
3. Create a new branch, e.g., named `changes-to-readme`.
4. Make changes to your files on this branch and commit them with a message. Push the changes.
5. Open a pull request and review your changes.
6. Merge the pull request and pull the `main` branch again. Verify that your changes have been merged.


## Repo Structure

After you've completed the previously described steps, please remove the content above. Include the following information in this readme file:

### Causal Capabilities of LLMs in June-Juli 2024

- an overview of the Digital Causality Lab (DCL) case studies is available [here](https://github.com/DigitalCausalityLab/causal-case-studies/issues)

### Participants
- Alexander Lorenz
- Jannik Svenson
- Lucas Mandelik

### Abstract

- [ ] Insert a brief description of the goals and results of your case study (around 250 words, English)
- [ ] You can upload and include figures, too

### Current State and Call for Extension

- [ ] Briefly summarize the state of your data product as of the end of the course
- [ ] Briefly summarize what could be added or improved in the future


## Organization of the Repo

We'd recommend you to organize your repo as follows.

* Include figures (`.jpg`, `.png`, ...) in a subdirectory called `figures/`, see [this example](figures/logo.png)
* Include data files (`.csv`, `.rda`, ...) in a subdirectory called `data/`, see [this example](data/experiment_data_counterfactual.rda)
* Include your R code (`.R` files) in a subdirectory called `R`, see [this example](R/my_function.R)
* In case you use quarto for your data product, include your `.qmd` files here, see [this example](demo_repo.qmd)

These basic recommendations are intended to give you a bit structure. You can deviate from them as you like but please make sure others should be able to understand what you did. 😄

# DCL Project

## Beschreibung
Eine kurze Beschreibung des Projekts.
Während des Data Science Moduls Kausale Inferenz wurden wir ermutigt ein eigenes Data Science Projekt durchzuführen. Dieses Repository enthält unsere Arbeit, welche nachfolgend einmal kurz eingeführt wird.

## Autoren
- [lucas.mandelik@studium.uni-hamburg.de](mailto:lucas.mandelik@studium.uni-hamburg.de)
- [alexander.lorenz@studium.uni-hamburg.de](mailto:alexander.lorenz@studium.uni-hamburg.de)
- [jannik.svenson@studium.uni-hamburg.de](mailto:jannik.svenson@studium.uni-hamburg.de)

## Datum
Datum der letzten Aktualisierung: 26. Juni 2024

## Inhaltsverzeichnis
1. [Einleitung](#einleitung)
2. [Grundlagen](#grundlagen)
3. [Parrots Paradox](#parrotsparadox)
4. [Beitrag](#beitrag)
5. [Schlussbetrachtung](#schlussbetrachtung)
6. [Lizenz](#lizenz)

## Einleitung
Eine detailliertere Beschreibung des Projekts, seiner Ziele und Funktionen.

## Grundlagen
Zuerst kann einmal festgehalten werden, dass wir uns im folgenden hauptsächlich mit dem nachfolgenden oft debattierten Paper: XXXXX beschäftigen.

## ParrotsParadox
hier das Paradoxon einleiten maybe mit IDS Knowledge

## Hauptteil
Wir haben uns dann weiterhin damit beschäftigt, wie die beiden Versionen von UHHGPT, nämlich ChatGPT 3.5 Turbo und ChatGPT 4 omni, die Bechmarks erfüllt, die das Paper vorgeschlagen hat.  

### Paper - Beispielfragen
Dazu haben wir zunächst die Fälle ausprobiert, die in dem Paper vorgestellt wurden. Dabei werden ChatGPT immer Sätze vorgelegt und darf immer nur mit "True" oder "False" antworten. Den ersten Fall und die Antwort von ChatGPT 3.5 Turbo kann man im folgenden Bild sehen:
<img src="LLM Fails\Edge Cases\Fail heights.png" align="center" width = "\textwidth" />
Da Bob Höhenangst hat, wäre die logische Konsequenz daraus, dass er bei der Wahl zwischen dem Riesenrad und dem Karussell das Riesenrad vermeiden würde. ChatGPT 3.5 Turbo ist in diesem Fall nicht dazu in der Lage gewesen, diesen kausalen Zusammenhang zwischen Höhenangst und dem Riesenrad zu ziehen, dass Bob durch das Riesenrad in die Höhe transportiert würde, was seine Höhenangst auslösen würde und er aus genau diesem Grund das Karussell dem Riesenrad vorziehen würde. ChatGPT 4 omni hingegen hat diesen Fall richtig gelöst.  
Tatsächlich sind wir dabei auch auf einen interessanten Fehler gestoßen. ChatGPT 4 omni hat bislang sehr gute Ergebnisse geliefert und hat bei keiner Frage, die wir ausgetestet haben, falsche Ergebnisse geliefert. So auch zuerst bei diesem Fall, der ebenfalls aus dem untersuchten Paper stammt:
<img src="LLM Fails\Academic Paper Cases\fish correct.png" align="center" width = "\textwidth" />
Da Sammy mit 10 Fischen rechnen würde, wäre er folglich bei 40 Fischen sehr erfreut und bei nur 5 Fischen vermutlich enttäuscht. Das hat ChatGPT 4 omni ohne Probleme hinbekommen. Interessanterweise ist uns aufgefallen, dass, sobald man den Namen von Sammy klein schreibt, ChatGPT 4 omni nicht mehr in der Lage ist, dies richtig zu lösen, wie man hier sehen kann:
<img src="LLM Fails\Academic Paper Cases\4.0 Fail.png" align="center" width = "\textwidth" />
Hier ist es also eventuell der Fall, dass ChatGPT nicht mehr in der Lage ist, zu identifizieren, dass es sich bei Sammy um eine Person handelt, weshalb hier dann kein logischer Zusammenhang erkannt werden kann.

### Eigene Ideen und bekannte Fälle
Desweiteren haben wir andere Fälle ausgetestet, die in der Vergangenheit aufgefallen sind, da ChatGPT sie nicht korrekt beantworten konnte und haben auch eigene Ideen ausgetestet, um zu prüfen, ob ChatGPT hier in der Lage dazu ist, kausale Zusammenhänge zu erkennen.  
Im ersten Beispiel geht es um das Thema Fußball:
<img src="LLM Fails\Edge Cases\3.5 Fail Fussball.png" align="center" width = "\textwidth" />
In diesem Fall ist ChatGPT 3.5 der Logik gefolgt, dass es hier eine einfache transitive Eigenschaft gibt, dass wenn Team A Team B besiegt und Team C Team A besiegt, Team C ja folglich besser sein müsste als Team B und somit auch Team B besiegen müsste. Dies ist allerdings beim Thema Fußball keine gegebene Eigenschaft, da die Teams verschiedene Spieltaktiken nutzen, die bei manchen Teams ein Schwachpunkt darstellen, von anderen Spieltaktiken jedoch ausgekontert werden. Das kann man z.B. auch gut in der EM betrachten. Deutschland hat z.B. 5:1 gegen Schottland gespiel. Da Schottland 1:1 gegen die Schweiz gespielt hat, müsste aus der Logik von ChatGPT 3.5 Deutschland auch deutlich gegen die Schweiz gewinnen, hier kam jedoch nur ein knappes Unentschieden zustande. Auch hier hat ChatGPT 4 omni jedoch die Nase vorne und konnte auch diese Frage richtig beantworten.  
Ein weiteres Beispiel kann hier gesehen werden:
<img src="LLM Fails\Edge Cases\Fail Box.png" align="center" width = "\textwidth" />
In der Fragestellung wird formuliert, dass es in einer blauen Box ein Apfel und eine rote Box mit einem Deckel gibt. Einem Menschen würde dabei sofort auffallen, dass folglich der Apfel einfach aus der blauen Box entnommen werden kann. ChatGPT 3.5 Turbo hingegen hat es hier jedoch nicht geschafft, diesen Zusammenhang zu erkennen - wir vermuten, dass das der Fall ist, da so genau beschrieben wurde, dass die rote Box einen Deckel hat, und dieser roten Box deswegen ein zu großer Wert für die Beantwortung der Frage beigemessen wurde.  
Auch hier konnte ChatGPT 4 omni jedoch korrekt antworten und hat darauf hingewiesen, dass die rote Box gar keine Rolle spielen würde, wenn man an den Apfel gelangen möchte. 

