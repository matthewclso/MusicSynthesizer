# MusicSynthesizer

This project attempts to synthesize recordings by learning from scores + recordings of existing classical music.  The idea is that if we give it enough scores and corresponding recordings, it will learn how to apply musicality to music.  Essentially, teaching a machine to play msuic.

It uses an implementation of the self-organizing map to "classify" every note in a music score.  It then uses a generic music synthesizer to generate a "robotic" recording.  Then, it uses dynamic time warping to map all these notes to the notes in a real recording.  It will then calculate a "difference" between the notes in the generic recording and the notes in the real recording (volume, tone, etc.).  This difference is then learned - hopefully being able to apply to test music scores and generic recordings, applying human-like musicality to them.

This runs on a Google Colab instance working off of Google Drive (it has just been imported to github for visibility). Feel free to use, just make sure to configure directory locations so they work for your environment.

This project uses the MusicNet dataset from UW CSE.  You can find more here - https://homes.cs.washington.edu/~thickstn/musicnet.html
