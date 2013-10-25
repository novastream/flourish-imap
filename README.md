flourish-imap
=============

Improved imap library from flourish, also with a simple Codeigniter loader


Added functions:
*Sorting, when calling listMessages you can sort the messages by newest or default = oldest
*When using IMAP you can fetch IMAP flags like /SEEN /DELETED /ANSWERED
*You can call countMessages and it will return the message count of the provided inbox
*Selectable inbox, default is INBOX but you can simply call eg. INBOX.SENT, SENT, INBOX.DRAFT and so on


Count messages by simply call:
$mailbox->countMessages()

if like above the function will count INBOX


Get/Fetch messages by using listMessages($limit=NULL, $page=NULL, $order='newest', $folder=NULL)

Where null values isn't set and default is used.