# 3D Social Media Effect

### Function @mixin to loop element in list
`
/**
    brief: loop child element in list and set content for it, check if :after set background
    $index: numer of element in list
    $isAfter: check is :after or not
*/
@mixin child-content($index, $isAfter) {
    @if $index == 1 {
        content: '\f09a';
        @if $isAfter {
            background: #3b5999;
        }
    }
    @else if $index == 2 {
        content: '\f099';
        @if $isAfter {
            background: #55acce;
        }
    }
    @else if $index == 3 {
        content: '\f0d5';
        @if $isAfter {
            background: #dd4b39;
        }
    }
    @else if $index == 4 {
        content: '\f0e1';
        @if $isAfter {
            background: #0077b5;
        }
    }
    @else if $index == 5 {
        content: '\f16d';
        @if $isAfter {
            background: #e4405f;
        }
    }
}`

### To use @mixin, let use @include
`@for $i from 1 through 5 {
    &:nth-child(#{$i}) {
        a {
            span {
                &:before {
                    @include child-content($i, false);
                }
                &:after {
                    @include child-content($i, true);
                    color: $bg-white;
                }
            }
        }
    }
}
`
