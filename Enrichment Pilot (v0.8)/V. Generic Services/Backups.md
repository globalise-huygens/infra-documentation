tba

Some first notes. Currently (23/11/23) the v1 HTR in the TextRepo exists in back-up form in CI's infrastructure as follows (about 75GB per copy):

On "Storage Flex Disk":

/backup

last backup, 1 copy
monthly, 1+1 unique copy (i.e. two unique files)
weekly, 1+1 unique copy
daily, 3+2 unique copies (i.e. 3 identical files, and 2 identical files)

The number of unique vs. identical copies above is obviously dependent on if and when the underlying Postgres database dumps changed. 

/data

5x, same file

Thus 15 instances (not copies..) of the HTR in different places, at €1,24/GB/yr =  €1,395 / year. However, it's really more than that, since separate copies are also being sent to tape at SurfSara. So, as a rough guess, say €1,500 / year. Now, with the second set of HTR, this will double. And, with a new set of documents in the TextRepo (i.e. files with known document boundaries, themselves constituted out of files), it will triple.

Clearly, there is room here for some efficiencies. The data on the [[Project Data (HuCDrive)]] is being backed-up as well, but I didn't get figures for this yet.