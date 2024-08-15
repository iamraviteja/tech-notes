# PR Checklist

This is **PR Checklist** for developing **React** and **NextJS** applications. References for compiling the list are given in the references section
> **Version:** 1.0.0

## List
1.  Do not hardcode config values or feature check values. Add the values in a constants file or pick values from environment file with good defaults in constants file.
2.  Folder structure : follow a consistent and logical grouping of files
    1.  Components
    2.  Layout & Views
    3.  State management
    4.  Library :  helpers functions, constants, 3rd party configs ( router, state config, analytics config)
3.  Create components :  Create components based on
    1.  Re use-ability
    2.  Providing clear encapsulation of different sections
4.  Avoid using unnecessary divs, use React Fragments instead
5.  Avoid giving layout styles like  spacing(margin, padding),  flex box layout to re useable components.
    1.  Provide a wrapper div to hold the layout styles.
    2.  Provide a class prop to inject the layout styles.( use ‘cn’ function of tailwind)
6.  Use Typescript in project [https://react-typescript-cheatsheet.netlify.app](https://react-typescript-cheatsheet.netlify.app)
    1.  Types for data objects : API responses, app states
    2.  Types for component props
7.  Keep your components dumb or simple.
    1.  Any calculation needed for component needs to be abstracted away.
    2.  Use props for actions, values to make component simple.
    3.  Use derived state in components.
    4.  Use {children} feature to compose components if component is immediate child.
    5.  Use context for state management with components.
8.  Use function to access prev state in useState. This will avoid issues with closures and batching.
9.  Don’t pass useState setter functions in case of passing action function to components. Pass a handler function to handle action logic in parent.
    1.  Naming convention for action prop ‘onActionHandler’.
10. Use useMemo, useCallback, React.memo for optimisation & caching. 
    1. Use useCallback and memoize component with React.memo for better results
    2. Use useMemo for objects, arrays in the component that will be passed as props to child components.
    3. Derived state should be wrapped in useMemo with state dependency.
12. Use states carefully don’t create multiple states.
    1. Use single union type instead of multiple states.
    2. Keep track of active or selected item by its id don’t duplicate the whole object. This ensures single source of truth for data.
13. Use the URL for states like filters, pagination but not useState.
    1. This makes the link a bookmark.
14. Make sure the useEffect has mostly a single dependency
    1. Use the clean up function to remove any event listeners and cancel api calls.
15. Consider React Query for caching api calls and api management.
   1. NextJS has caching out of the box (this point needs review)
16. Re usability :
   1. Re use markup, create component
   2. Re use state, create custom hook
   3. Re use logic , create utility function

## References
Below are the references used to compile the list based on version.

### Version 1.0.0
[ByteGrad 17 React best practises](https://www.youtube.com/watch?v=5r25Y9Vg2P4)

