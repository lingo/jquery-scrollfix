# jQuery ScrollFix 1.0

jQuery plugin to fix an element based on current scrolling position of the page.

## Browser support

Tested in Firefox, Google Chrome, Safari, Opera and MSIE 7+

## Usage

The plugin provides single jQuery method you can use.

### `$(containerSelector).scrollFix(elementSelector, options);`

Custom CSS is required for this to have effect:

    containerSelector.scroll-fix {
        height: <insert value here>px; /* Ensure that the container has height when the element is fixed */
    }

    elementSelector.scroll-fix {
        position: fixed;
        top: 0;
    }

See [demo.html](demo.html) for an example.


## Options

<table>
  <thead>
    <tr>
      <th>
        Name
      </th>
      
      <th>
        Default
      </th>
      
      <th>
        Description
      </th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <th>
        scroller
      </th>
      
      <td>
        window
      </td>
      
      <td>
        element to watch for scrolling events
      </td>
    </tr>

    <tr>
      <th>
        elementFixClass
      </th>
      
      <td>
        scroll-fix
      </td>
      
      <td>
        class added to the element when it is supposed to be fixed
      </td>
    </tr>

    <tr>
      <th>
        containerFixClass
      </th>
      
      <td>
        scroll-fix
      </td>
      
      <td>
        class added to the element's container when it is fixed
      </td>
    </tr>

    <tr>
      <th>
        fixBoundaryOffset
      </th>
      
      <td>
        0
      </td>
      
      <td>
        offset aplied when detecting whether to fix the element
      </td>
    </tr>

    <tr>
      <th>
        unfixBoundaryOffset
      </th>
      
      <td>
        0
      </td>
      
      <td>
        offset aplied when detecting whether to unfix the element
      </td>
    </tr>
  </tbody>
</table>