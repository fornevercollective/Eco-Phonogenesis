# Visual Map of Mouth Shapes and Phoneme Embeddings

## Overview
This artifact maps human phonemes to mouth shapes and provides a conceptual framework for universal phoneme embeddings. Animal phonemes are approximated based on vocal tract similarities. The map is designed to be visualized as a table or diagram, with mouth shapes described for each phoneme category.

## Mouth Shapes and Corresponding Phonemes

Phonemes are categorized by articulatory features (place and manner of articulation). Below is a table mapping mouth shapes to human phonemes, with notes on animal approximations.

| Phoneme Category | Example Phonemes | Mouth Shape Description | Animal Approximation |
|------------------|------------------|-------------------------|----------------------|
| **Bilabial** (lips together) | /p/, /b/, /m/ | Lips fully closed, then released (/p/, /b/) or held with nasal airflow (/m/). | Similar in mammals (e.g., primate grunts, dog barks). |
| **Labiodental** (lip-teeth) | /f/, /v/ | Lower lip touches upper teeth, air escapes between. | Rare in animals, approximated in some primate vocalizations. |
| **Dental/Alveolar** (tongue-teeth/ridge) | /t/, /d/, /s/, /z/, /n/ | Tongue tip at teeth (/θ/, /ð/) or alveolar ridge; lips neutral or slightly parted. | Common in mammal vocalizations (e.g., cat hisses for /s/-like sounds). |
| **Palatal** (tongue-palate) | /j/, /ʃ/, /ʒ/ | Tongue near hard palate; lips rounded or neutral. | Approximated in bird calls (e.g., parrot mimicry). |
| **Velar** (tongue-velum) | /k/, /g/, /ŋ/ | Back of tongue at soft palate; lips neutral. | Common in mammal growls (e.g., big cats). |
| **Glottal** (throat) | /h/, /ʔ/ | Open mouth, airflow from throat; minimal lip movement. | Universal in animal vocalizations (e.g., hoots, roars). |
| **Vowels** (open tract) | /i/, /a/, /u/ | /i/: Lips spread, tongue high. /a/: Mouth open, tongue low. /u/: Lips rounded, tongue back. | Approximated in primate calls (e.g., gibbon songs) or whale vocalizations. |

### Visualization Notes
- **Table Format**: Use the above table for a textual map. Columns: Phoneme Category, Example Phonemes, Mouth Shape, Animal Approximation.
- **Diagram Option**: Create a sagittal view of the vocal tract (side profile) with annotations for each phoneme’s articulation point (lips, tongue, etc.). Overlay mouth shape icons (e.g., closed lips for /m/, rounded lips for /u/).
- **Animal Phonemes**: Since animals lack standardized phonemes, use spectrogram similarities (e.g., dog barks resemble bilabial stops, bird trills resemble alveolar trills).

## Universal Phoneme Embeddings

Phoneme embeddings are high-dimensional vectors capturing acoustic and articulatory features. Below is a conceptual framework for universal embeddings, assuming a model like wav2vec or IPA-based encoding. Actual embeddings would be numerical (e.g., 512-dimensional vectors) but are described qualitatively here.

| Phoneme | Embedding Features | Description |
|---------|--------------------|-------------|
| /p/ | [+bilabial, -voiced, +stop] | High lip closure energy, short burst, no vocal fold vibration. |
| /b/ | [+bilabial, +voiced, +stop] | Same as /p/ but with vocal fold vibration. |
| /m/ | [+bilabial, +voiced, +nasal] | Lip closure with nasal resonance. |
| /f/ | [+labiodental, -voiced, +fricative] | Lip-teeth friction, continuous airflow. |
| /s/ | [+alveolar, -voiced, +fricative] | Tongue at ridge, hissing airflow. |
| /i/ | [+high, +front, +vowel] | High tongue, spread lips, bright formants. |
| /a/ | [+low, +open, +vowel] | Open jaw, low tongue, wide resonance. |
| /u/ | [+high, +back, +rounded, +vowel] | Rounded lips, back tongue, low formants. |

### Embedding Notes
- **Features**: Include place, manner, voicing, and formant frequencies (F1, F2 for vowels).
- **Universality**: Use IPA as a basis for cross-linguistic consistency. Animal vocalizations can be mapped to similar features (e.g., dog bark: [+bilabial, +stop]).
- **Implementation**: In practice, embeddings are learned via neural networks (e.g., wav2vec 2.0) trained on multilingual speech data. Here, we simulate with descriptive features.

## Animal Phoneme Approximations
Animals don’t use phonemes like humans, but their vocalizations can be mapped to human-like articulatory categories:
- **Primates**: Grunts (/p/, /b/), screams (/a/, /i/).
- **Canids**: Barks (bilabial stops), howls (vowel-like /u/, /a/).
- **Felids**: Hisses (/s/), roars (glottal /h/, open vowels).
- **Birds**: Trills (alveolar-like), whistles (vowel-like).
- **Cetaceans**: Clicks (stop-like), songs (vowel-like formants).

## Usage
- **Visualization**: Render the table as an HTML page or use a tool like Matplotlib for a diagram (code available upon request).
- **Embeddings**: Use the feature descriptions as input for a speech synthesis or recognition model.
- **Extensions**: Add spectrogram images for each phoneme or animal sound for a richer map.