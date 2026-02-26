# Portable-GNSS-Software-Defined-Receiver-Based-on-ADALM-Pluto-SDR

This repo is a reproducible install recipe for:
- Ubuntu 20.04 (focal)
- GNU Radio from apt (3.8.1.0, prefix **/usr**)
- libiio v0.25 (source -> /usr/local)
- libad9361-iio (0.2)
- gr-iio / gnuradio-iio 0.3 (ADI branch upgrade-3.8)
- GNSS-SDR (next) built with Pluto support

## Quick start
```bash
git clone <YOUR_REPO_URL>
cd gnss-sdr-pluto-ubuntu20.04-gnuradio3.8-iio

bash install/00_prereqs.sh
bash install/10_check_gnuradio_prefix.sh

bash install/20_build_libiio_v0.25.sh
bash install/30_build_libad9361_iio.sh
bash install/40_build_gr_iio_upgrade3.8.sh
bash install/90_pluto_check.sh

bash install/50_build_gnss_sdr_next_pluto.sh
