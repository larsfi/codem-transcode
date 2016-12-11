## codem-transcode 0.5.11 (2015/12/02) ##

* Sanitize null values (@brain64bit)
* Allow HTTPS for notification delivery (@mirion)

## codem-transcode 0.5.10 (2015/09/16) ##

* Increase maxBuffer to 4MB to compensate for older ffmpegs

## codem-transcode 0.5.9 (2015/09/03) ##

* Fix for lingering "processing" jobs. (#42)
* Encoder options can be an array instead of a string as well (to allow complex filters)

## codem-transcode 0.5.8 (2015/07/05) ##

* Prevent transcoder from returning a negative freeSlot count (@larsfi).

## codem-transcode 0.5.7 (2015/04/23) ##

* Add option for database port in config (@brain64bit).

## codem-transcode 0.5.6 (2015/04/22) ##

* Return a job from memory if it is still transcoding.

## codem-transcode 0.5.5 (2014/09/08) ##

* Added basic HLS support (@cutalion) using "segments_options".

## codem-transcode 0.5.4 (2014/03/18) ##

* Updated sqlite3 dependency to 2.2.0.

## codem-transcode 0.5.3 (2014/01/27) ##

* Bugfix: issue #19 and #20, missing or corrupt ffmpeg will no longer put transcoder in weird state.
* Send "X-Codem-Notify-Timestamp" header for notifications with millisecond precision (instead of second).

## codem-transcode 0.5.2 (2013/09/10) ##

* Bugfix: migrations should create "Jobs" table (instead of "jobs")

## codem-transcode 0.5.1 (2013/07/08) ##

*   Extra path separator / nul file check for platform-specific issues (Windows/*nix)
*   Allow thumbnail-only jobs. See README.

## codem-transcode 0.5.0 (2013/07/02) ##

*   All fixes/features from the betas.
*   Use async package for some of the complex callback chains.
*   Ability to capture thumbnails from the videos after transcoding.

## codem-transcode 0.5.0-beta.4 (2013/04/30) ##

*   Fix for #15, cannot open database when using default config.
*   sqlite3 dependency updated to 2.1.7.

## codem-transcode 0.5.0-beta.3 (2013/04/25) ##

*   Allow purging of old successful jobs. See README for usage.
*   Tested against Node.js 0.10.

## codem-transcode 0.5.0-beta.2 (2013/03/07) ##

*   Switch to Sequelize for database abstraction. codem-transcode now supports SQLite, MySQL and Postgres. PLEASE NOTE
    that this change is *not* backwards compatible. You will need to update your database. If you are coming from an old
    version of codem-transcode we advise you to move away your old database and let the software generate a new database
    for you.
    
## codem-transcode 0.5.0-beta.1 (2013/02/19) ##

*   The logging system should now be more able to handle unexpected issues, such as when your logging file system is out
    of space. In most cases the system should be able to gracefully intercept any issues and resume operation after the
    issue has been cleared (ie. more space has been created).

## codem-transcode 0.4.4 (2013/01/28) ##

*   Use a "=" instead of a "LIKE" when loading a job. Prevents excessive disk IO.

## codem-transcode 0.4.3 (2013/01/22) ##

*   Allow both time formats in the ffmpeg output parsing (xx:xx and xx:xx:xx).

## codem-transcode 0.4.2 (2013/01/07) ##

*   Fix for copying a file across partitions.

## codem-transcode 0.4.1 (2012/10/16) ##

*   Added ffprobe support.

## codem-transcode 0.4.0 (2012/10/10) ##

*   Updated package to Node 0.8.

## codem-transcode 0.3.1 (2012/06/27) ##

*   Allow disabling of scratch directory.

## codem-transcode 0.3.0 (2012/03/20) ##

*   Updated dependency to a newer version of Node.
*   Update ffmpeg time parsing.
*   Switched from connect to express.

## codem-transcode 0.2.1 (2011/09/26) ##

*   Add additional "X-Codem-Notify-Timestamp" HTTP header.

## codem-transcode 0.2.0 (2011/08/23) ##

*   Deleting and cancelling jobs.
*   Additional error checking.

## codem-transcode 0.1.2 (2011/07/11) ##

*   Additional logging.
*   Notify when duration is known.
*   Added extra check when creating directories.

## codem-transcode 0.1.1 (2011/05/24) ##

*   Fixed license info

## codem-transcode 0.1.0 (2011/05/24) ##

*   Initial release