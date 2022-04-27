### Server
the mysql will act as copy storage for all conversation between _AI_ $\to$ _user_
and between _user_ $\to$ _user_.  Since the data will never be changed and strictly be read from and addded on to there is no reason to have Mongo for this task. this data will later be feed into the machine learning comp