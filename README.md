# CIS-PD-MUSC

'annotate and clip videos.ipynb'
    Downloads cycle videos, annotates activities by frame number, and clips into activity videos.



'mp4 metadata extract.ipynb
    Extracts the timestamp metadata for the cycle videos that are in mp4 format.

    When cross referencing watch shaking time on form 509 with video timestamp metadata, the following discrepancies are found:
    Summary of data that is off
    - 1003 is off by 1 yr and 5 hours and some seconds, cycle 3 was off by an additional 9 min
    - 1030 is off by several seconds (usually around 30 sec)
    - 1005 is off by 1 yr 5 hrs and some seconds, cycle 2 is off by an additional 5 min
    - 1007 is off by 1 yr 5 hrs and some seconds
    - 1009 is off by 1 yr 5 hrs and some seconds
    - 1019 is off by 29.5 min
    - 1024 is off by 50 sec
    - 1048 cycle 1 3.5 hours off, cycle 2 missing, cycle 4 is 4 hrs off, cycle 5 is about 4 hrs off
    - 1050 is off by 1 yr, 5 hrs and some sec

    These videos we suspect editing, so Skip these subjects:
    - 1023 is off by 18 days, but the watch shaking time for all cycles the same
    - 1039 is off by 2 months, 13 days, and variable time but the watch shaking time for all cycles the same
    - 1043 is off by 2 months, 1 day, but  the watch shaking time for all cycles the same



'sync accelerometer to video clips.ipynb'
    For each subject/cycle/activity, take video frames and convert to UTC timestamp using mp4 metadata.
    Compared watch shaking time and adjusted UTC timestamps by offset for UAB site.
    Did not include subject 1048 data since all videos were already clipped by activity.