function wps_change_role_name() {
global $wp_roles;
if ( ! isset( $wp_roles ) )
$wp_roles = new WP_Roles();
$wp_roles->roles['subscriber']['name'] = 'Новичок';
$wp_roles->role_names['subscriber'] = 'Новичок';
}
add_action('init', 'wps_change_role_name');
