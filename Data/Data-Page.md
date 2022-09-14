# Data Page

At times, when we need to access data (say Employee details), we need to get data from a database. But, reaccessing it every time we need it isn't a good practice. So, to avoid this performance degradation, we use data pages in PEGA. Data Pages will query a database, and the result (whether a list or a single record) is cached as a 'page'.

There are three types of data pages:

- Single (one record)
- List (more than one record)
- Savable (this type handles database insertion, or persistence)

Data Pages are instances of the Rule-Declare-Pages class. The name of a data page starts with the prefix D_. On the clipboard, the contents of data page instances are visible but are read-only.

<img src="https://res.cloudinary.com/practicaldev/image/fetch/s---ppZRdls--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/hkb9fbpzfu8bzgtzwb13.png" alt="data page" />

Scope of data page:
1. Node- If the Scope of a Data Page is specified as Node, it is shared across all the requestors of that node.

2. Requestor- If the Scope of a Data Page is specified as Requestor, it can be accessed by all the threads opened by the requestor.

3. Thread- If the Scope of a Data Page is specified as a Thread, it can be accessed only by that particular thread.
