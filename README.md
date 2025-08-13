# Injection Campaign

This repository contains the files relevant to the work summarized in [this manuscript](https://arxiv.org/abs/2506.19990)

## Contents

This repository is divided into three directories: 
 1) config_files: contains most of the relevant configuration files for launching the parameter estimation (PE) jobs in parallel bilby
 2) data: lists the intrinsic parameters or the 30 SXS simulations injected in the main part of the work.
 3) posteriors: contains the parameter posteriors for all the relevant parameter estimation runs.

In more detail, dirs 1) and 3) have

### config_files

This subdir contains two subdirs: one has all the config files for the inspiral-merger ringdown consistency tests (IMRCT) and the other has the config files for the injection-recoveries carried out using individual waveform models. Each of these two subdirs are further decomposed into three subdirs each named after the model used in the injection recovery. The three subdirs under the IMR_consistency subdir are further separated into MODEL_inspiral and MODEL_mr subdirs, where MODEL = SEOB or TPHM or XPHM.

### posteriors

This subdir contains all the relevant posteriors from the PE jobs. In particular, it has three subdirs corresponding to the three main results sectoins of the manuscript linked above. The subdir Three_Model_Injections contains the results pertaining to Sec. IV of the manuscript where 35 numerical relativity injections were recovered with the models SEOB, TPHM and XPHM. Accordingly, this subdir has three subdirs named after these models. Each one contains 35 text files named after either the SXS or BAM simulation catalog ID. Each file format is as follows
  [chirp_mass, small mass ratio, a1, a2, tilt1,tilt2, Delta_phi, right ascension, declination]
