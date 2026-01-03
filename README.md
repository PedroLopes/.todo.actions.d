# .todo.actions.d
Custom actions for todo.txt CLI (todo.sh), including a variant that opens dokuwiki-based links rather than only http ones.


## open

Running ``todo.sh open <number_of_todo_item>`` will trigger the ``open`` script, which is virtually identical to the popular ``nav`` action (finds and opens URLs inside your todo item) but can also search and open DokuWiki links, defined simply as ``[[page_id]]``. Obviously the ``nav`` command can already open a dokuwiki link if you provide the full URL like ``https://www.dokuwiki.org/plugin:nspages`` but using ``open`` allows you to set a ``$WIKI_BASEPAGE_URL`` variable (e.g., ``export $WIKI_BASEPAGE_URL="https://www.dokuwiki.org/"``) so that when you would open a item that simply contains ``[[plugin:nspages]]`` it will actually open the full link. This allows to write shorter todo entries that are compatible with dokuwiki pages (niche use case but see [todotxt2tododokuwiki](https://github.com/PedroLopes/todotxt2tododokuwiki) if you want a tool that syncs your todo.txt with a dokuwiki page). 

## edit

Original edit action. 
