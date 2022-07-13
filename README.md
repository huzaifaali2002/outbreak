# Detecting outbreaks before they become endemic

This project was an entry to Rice Datathon 2022.

Using Twitter API to generate 2010 tweets, we created a dataset of swine flue and corresponding symptoms' mentions on Twitter. Using spatiotemporal dot distributions on chloropleths of USA we aimed to confirm our hypothesis of twitter mentions of swine flue being correlated with the actual pandemic itself.

After confirming our hypothesis, we built a tool in Shiny that lets users search for potential outbreaks happening in their region and telling them the precautions they can take to keep themselves safe. We define a disease as a collection of its constituent symptoms, and the tool looks for tuples of disease-related words in recent tweets which are occurring in the user's region at a frequency 2 standard deviations higher than the baseline frequency of the tuple. It then attempts to map the symptoms to a disease. If no disease is found correlated to a tuple of symptoms, it detects a potential new infectious disease being spread.

For more information on the project:
https://devpost.com/software/outbreak-4q3dxt
