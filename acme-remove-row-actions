<?php

/**
 * Plugin Name: Acme row actions filter
 * Plugin URI: https://github.com/acme-top/wordpress-remove-row-actions
 * Description: 禁用文章列表中的“快速编辑”功能
 * Version: 0.1
 * Author: Acme
 * Author URI: http://www.acme.top
*/

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

/*
 * 禁用文章列表中的“快速编辑”功能
 * 否则可能会导致 Markdown 格式的文章内容变为 HTML 代码
 */
add_filter( 'post_row_actions', 'acme_remove_row_actions', 10, 2 );

function acme_remove_row_actions( $actions )
{
    if( get_post_type() === 'post' ) {
		  unset( $actions['inline hide-if-no-js'] );
    }
    return $actions;
}

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
