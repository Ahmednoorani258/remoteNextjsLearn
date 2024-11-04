practicing new things and exploring new feauters in this repo

#File Conventions

layout   	    Shared UI for a segment and its children
page	        Unique UI of a route and make routes publicly accessible
loading 	    Loading UI for a segment and its children
not-found	    Not found UI for a segment and its children
error	        Error UI for a segment and its children
global-error	Global Error UI
route	        Server-side API endpoint
template	    Specialized re-rendered Layout UI
default	        Fallback UI for Parallel Routes


# UsePathName 

You can use the usePathname() hook to determine if a nav link is active.

`way to use`

{import { usePathname } from 'next/navigation'
import Link from 'next/link'
 
export function NavLinks() {
  const pathname = usePathname()
 
  return (
    <nav>
      <Link className={`link ${pathname === '/' ? 'active' : ''}`} href="/">
        Home
      </Link>
        </nav>
  )
}}