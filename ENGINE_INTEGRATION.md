# Integrarea motorului vocal — următoarea etapă

## Motor recomandat
Sherpa-ONNX oferă runtime TTS offline pentru Android și suportă familii de modele precum Piper/VITS. Documentație: https://github.com/k2-fsa/sherpa-onnx

## Pașii tehnici rămași
1. Selectarea unei versiuni stabile a bibliotecii Android Sherpa-ONNX.
2. Adăugarea dependenței Android/AAR și a codului nativ pentru inferență.
3. Descărcarea/instalarea modelului românesc și a fișierului său de configurare.
4. Implementarea conversiei capitolului în fragmente, sintetizarea WAV-urilor și concatenarea lor cu pauze.
5. Adăugarea encoderului MP3 opțional.
6. Parser de EPUB; PDF text-selectabil; OCR separat pentru PDF-uri scanate.
7. Detectarea replicilor și editor pentru asocierea manuală a personajelor cu voci instalate.
8. Importul modelelor personalizate trebuie să verifice arhitectura, configurația, sursa și licența. Un fișier audio simplu nu este un model vocal.

## Limitarea modelelor
Catalogul standard Piper include modelul românesc `ro_RO-mihai-medium`, o voce masculină. Nu presupune că există deja o pereche feminină românească oficială. Pentru mai multe voci românești este necesar să verificăm modele compatibile și licențele fiecăruia.
