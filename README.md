# Olympic-Games-Simulation-using-Linked-Lists 🏅

## 📑 Description:
In this repository we will present our work in our first year as computer science engineering student at **ESI**, *"Ecole Nationale Supérieure d'Informatique"*, the document explaining it will be shared in the repo, it is in french.

**Here is a detailed description of what we were asked to implement in our project:**

### Title: Olympics Athletes Registration Management

### Problem statement:
 In this project, we want to organize and represent the registrations of athletes for the Olympic Games in a matrix structure of singly linked linear lists. It is assumed that there are a maximum of 200 events and 150 countries. The nbpays represented countries are listed in alphabetical order in a table called "tabpays". Similarly, the names of the nbépreuve planned events are listed in alphabetical order in a table called "tabépreuve". It is assumed that each country can present from 0 to 10 athletes in each event (maxathletes=10). The names of the athletes are listed in linked lists, with the heads included in the elements of a matrix "tabjo", whose row indices are the event numbers, column indices are the country numbers, and each element of "tabjo" is a structure of type "concurrents", containing a pointer to an unsorted linked list of the names of the athletes who participate in an event for a country (or NIL if there are none).

### Work required:
 In the first step, program the singly linked linear list model seen in class.
Write and program the following modules:

A procedure "creer_tabjo" that creates "tabpays" and "tabépreuve" as well as the matrix of linked lists "tabjo" containing the names of all athletes from all countries in all events. To quickly fill this structure, you can randomly generate, for each country, a number between 0 and 10 corresponding to the number of registered athletes for a given event. For each element of "tabjo", you can also randomly generate athlete names of up to 25 characters.

A procedure "inserath" (nomath: string; nump, nume: integer) that inserts a new athlete, defined by their name "nomath", country number "nump", and event number "nume". The insertion should only be done if the following two conditions are met for that country and event: there are fewer than "maxathletes" athletes already registered, and "nomath" is not already listed.

A procedure "listathpays" (pays: string) that lists the names of all athletes from a given country, sorted by event. You should display the name of each event for which at least one athlete from the country is registered, followed by the (unsorted) list of athlete names. If the country is not known, you should display an error message.

A function "sansath" (ne: integer): boolean that returns true only if no athlete is registered for the event number "ne", i.e., if the row "ne" only contains NIL values.

A procedure "listjo" that displays the complete content of the "tabjo" matrix, event by event: for each event in which at least one athlete is registered, we display the name of the event, followed by the name of each country that has registered competitors and the names of the registered athletes.

A procedure "suppays" (pays: string) that allows a country to be removed from the "tabjo" and "tabpays" structures following the announcement of its withdrawal.

*Benefits of implementing this project include efficient organization and management of athlete registrations for the Olympic Games, as well as the ability to easily add, remove, and search for athlete and country data.*

**- Libraries we have used:**
- stdlib.h
- stdio.h
- Windows.h
- conio.h
- time.h

*And we used e-speak in order to generate sounds.*

**PS:** This program is executable only on windows, because we used the *windows.h* library

## 📥 Setup:
#### - Build e-speak in order to play the sound in our program: 
check those ressources fo that: https://github.com/espeak-ng/espeak-ng/blob/master/docs/building.md#windows

#### - Install windows.h 
If you want to check whether MSVC is installed on your system and windows.h is available, you can try running the following command for windows in the bash shell:

``` echo "#include <windows.h>" | cl /c /EHsc - ```

#### - Install conio.h
Check those ressources for that: https://github.com/thradams/conio
