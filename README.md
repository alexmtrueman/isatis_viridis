# Viridis colour palette for Isatis #

The Python 2D plotting library [`matplotlib`](http://matplotlib.org/) changed its default colour palette from a rainbow-based scheme called 'jet' to a new scheme called 'viridis'. Viridis was designed to be:

- Perceptually uniform: no particular colour 'stands out' more than any other. This is important in scientific visualization to prevent artificial patterns or trends appearing in the data because one colour is more apparent to the human eye than another.
- Printable in grey-scale: if the colour palette happens to be printed or photocopied in grey-scale the highs and lows can still be identified. It is perceptually uniform in grey-scale as it is in colour.
- Colour-blind compatible: people with the most common forms of colour blindness should still be able to interpret visualizations using this colour palette.

In these three areas the new palette is superior to traditional rainbow-based palettes. You can read more about [viridis](http://bids.github.io/colormap/) or watch the [presentation](https://youtu.be/xAoljeRJ3lU), which has an interesting discussion of the theory.

I have created a series of viridis [palettes](https://github.com/alexmtrueman/isatis_viridis) for [Isatis](http://www.geovariances.com/en/isatis-all-in-one-software-for-geostatistics-ru324). There are several palttes with different numbers of colour levels (some Isatis processes may have difficultly with high numbers of levels). The 128-level palette should work in most instances but switch to 64 or 32-level palettes if you have trouble.

During the development of viridis three other colour scales were developed that have a more red appearance. I have included one of these "option c" in this reporitory. 

The palette files are in the ASCII export format used by Isatis. To import the palette go to `File->Color palettes...` and select `Import...` to import the ASCII file. You can now create viridis-based colour scales for visualising data. Alternatively run the journal file included in this repository ([journals](https://github.com/amt4158/isatis_viridis/tree/master/journals)) making sure that you modify the path variable.

If you are used to using rainbow colour palettes it can take a bit of getting used to a palette like viridis; however, I think after a while you will agree that it is superior.
