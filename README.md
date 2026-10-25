# VoceaVie Android — proiect de pornire

Aplicație Android pentru citirea romanelor în română, cu capitole, atribuirea vocilor personajelor și export audio.
Acesta este un **starter project**, nu un APK gata de instalat și nu include încă runtime-ul neural Sherpa-ONNX/Piper. Interfața și fluxul de import sunt punctul de pornire.

## Deschidere
1. Deschide folderul `VoceaVieAndroid` în Android Studio.
2. Lasă Gradle să sincronizeze proiectul.
3. Rulează pe un telefon Android.

## Ce include acest starter
- selectarea unui fișier TXT din telefon;
- împărțirea textului în capitole pe baza titlurilor uzuale;
- bibliotecă inițială de personaje și atribuirea manuală a replicilor;
- setări pentru voci și importarea fișierelor de model (`.onnx` și `.json`) în folderul privat al aplicației;
- arhitectură separată pentru motorul TTS.

## Important
Butonul de generare audio este marcat ca indisponibil până la integrarea runtime-ului neural. Nu folosește vocea Android ca fallback, deoarece aceasta a fost problema prototipului anterior. Pentru generare locală, integrarea planificată este Sherpa-ONNX cu un model românesc compatibil. Modelul `ro_RO-mihai-medium` este o voce masculină; trebuie verificate separat modelele feminine și licențele lor.

## Formate
În această primă etapă este implementat importul TXT. EPUB și PDF cu text selectabil sunt etape următoare. PDF-urile scanate necesită OCR.
