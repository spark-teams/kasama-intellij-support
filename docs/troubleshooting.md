# Troubleshooting

In case you experience problems with Kasama, you can find answers to specific problems below.
If your problem persists, please [open an issue](https://github.com/spark-teams/kasama-intellij-support/issues/new/choose).

## IDE Logs

Kasama logs potential problems in the IDE log, which you can find at **Help > Open Log in Editor**.

## Kasama Plugin not started, failed to obtain database lock

You cannot use Kasama in multiple IDEs opened in parallel sharing the same Kasama database.
Hence, on IDE startup, Kasama checks if the database is already used by a different IDE instance.
In order to use Kasama in the second IDE instance, either close the other IDE or use a different data folder.

To change the data folder, navigate to **Settings... > Tools > Kasama**. In the **Advanved** section, set a different data folder
in the **Data Folder** field.

Note that different locations of Kasama tracking data cannot be joined together at the moment.

## Kasama Plugin not started, database is not valid

This error means that the database is in an invalid state. This can occur, if a database is shared across different IDEs with different Kasama plugin installations,
or if the file has been changed manually.

Please use a different data folder path.

If you think the invalid database is due to a bug, please [open an issue](https://github.com/spark-teams/kasama-intellij-support/issues/new/choose).
