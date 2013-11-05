************
Introduction
************

:Date: 05 November 2013
:Authors: Thomas V. Wiecki, Michael J. Frank
:Contact: thomas.wiecki@gmail.com
:Web site: http://github.com/twiecki/bg_inhib
:Paper: http://ski.clps.brown.edu/papers/WieckiFrank_psyrev.pdf
:Copyright: This document has been placed in the public domain.
:License: Simplified BSD
:Version: 1.1

This is the neural network model and accompanying scripts to run and
analyze the model presented in:

"A computational model of inhibitory control in frontal cortex and
basal ganglia." Wiecki, T.V. & Frank, M.J., Psychological Review, 2013

To run the selective response inhibition simulations:

::

  python emergent.py --run -b 4 -g saccade


To run the stop-signal simulations:

::

  python emergent.py --run -b 4 -g stopsignal

This should populate the logs directory. After this is finished (might
take quite some time), run:

::

  python emergent.py --analyze -b 4 -g saccade
  python emergent.py --analyze -b 4 -g stopsignal

This should populate the plots subdirectories. Note that plots used in
the final paper are often edited to improve quality.

