1. I have rewrited search function to use db_select instead of db_query because it would be much more easy to support (although a little slower)
2. Replaced search by node_revision to search by node
3. I don't want to use views here, because by my experience it will greatly reduce performance for many nodes, so we need to modify the main search function to support my code further
4. Added a little trick with hook_menu: page arguments - 'mysearch/%'
5. Delivered the title to drupal_set_title function.

Example: http://drupal7.2st.biz/mysearch/example