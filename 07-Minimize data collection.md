# Sheet n°7: Minimize data collection

#### You shall only collect personal data that is adequate, relevant and necessary in relation to the purposes for which they are processed, as defined at the time of collection.

## Before collection, think about the different types of data you need to collect and try to limit your collection to what is strictly necessary.

* Think about the different **types of data** that will need to be collected before an application is implemented and **document** this thinking.

* If specific data is not **needed for a certain category of people**, do not collect it.

* Process and store data in a way that **reduces accuracy** (similar to pseudonymization). For example, store only the year of birth instead of a full date of birth if the application only needs the year.

* If collecting particularly sensitive data, such as health or criminal convictions data, be sure to collect only the **minimum required**. Due to the regulatory constraints, the simplest solution is still to **not collect them** if you can do without them.

* Minimize the amount of data collected also in the **log data** and do not store sensitive or critical data (health data, passwords, etc.).

* Some features may improve the user experience, but are **not strictly necessary for your application to work properly** (e.g. geolocation to simplify a geographic search). In this case, the end user must be able to **choose whether or not to use** this functionality. If he uses it, the data that you are led to collect for its operation must only be kept for the time strictly necessary for its operation and never be used for other purposes.

* Remember to associate **retention periods** for each category of data, depending on the purpose of the processing and the legal or regulatory obligations relating to their retention. Logs must also have a retention period. Document the defined retention durations. You will need to be able to justify them.

## Once the data has been collected, set up automatic deletion mechanisms.

* Implement an automatic **purge** system at the end of the shelf life. You can also implement manual reviews of stored data on a periodic basis.

* To ensure complete erasure, erase **physically** all data that is no longer needed using specialized tools or by destroying the physical media.

* If the data is still useful, you can reduce its sensitivity by using **pseudomisation** or even **anonymisation** methods. In case of pseudonymization, these data remain subject to the regulations on personal data (see [Sheet 1](#Sheet_n°1_:_Identify_personal_data)).

* Log the **automatic deletion procedures**. The corresponding logs can be used as a **proof of deletion** of a data item.
