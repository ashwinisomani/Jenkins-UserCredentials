#CSRF protection support
function is_crumbs_enabled() {
  use_crumbs="$( $CURL -s ${JENKINS_WEB}/api/json?pretty=true 2> /dev/null | python -c 'import sys,json;exec "try:\n  j=json.load(sys.stdin)\n  print str(j[\"useCrumbs\"]).lower()\nexcept:\n  pass"' )"
  if [ "${use_crumbs}" = "true" ]; then
    return 0
  fi
  return 1
}

#CSRF protection support
function get_crumb() {
  ${CURL} -s ${JENKINS_WEB}/crumbIssuer/api/json | python -c 'import sys,json;j=json.load(sys.stdin);print j["crumbRequestField"] + "=" + j["crumb"]'
}

