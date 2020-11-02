<?php
$data = <<<EOF
copy
6407b0e94181790501fd1e167b474872
1081e37283d90000800003c07f3ef6bf
82, 12

pointer
hand
hand2
9d800788f1b08800ae810202380a0822
e29285e634086352946a0e7090d73106
82, 12

default
left_ptr
right_ptr
draft_large
draft_small
arrow
82, 12

link
640fb0e74195791501fd1ed57b41487f
3085a0e285430894940527032f8b26df
82, 12

progress
left_ptr_watch
3ecb610c1bf2410f44200f48c40d3599
08e8e1c95fe2fc01f976f1e063a24ccd
82, 12

icon
dotbox
dot_box_mask
draped_box
target
80, 30

help
left_ptr_help
d9ce0ab605698f320427677b458ad60b
5c6cd98b3f3ebcb1f9c7f1c204630408
question_arrow
48, 48

grabbing
fleur
dnd-none
size_all
48, 48

grab
hand1
48, 48

alias
dnd-link
56, 33

cross
diamond_cross
crosshair
cross_reverse
48, 48

no-drop
dnd-no-drop
48, 48

not-allowed
crossed_circle
03b6e0fcb3499374a867c041f52298f0
# 48, 48

move
9081237383d90e509aa00f00170e968f
# 48, 48

col-resize
ew-resize
h_double_arrow
sb_h_double_arrow
size_hor
14fef782d02440884392942c11205230
028006030e0e7ebffc7f7070c0600140
# 48, 48

row-resize
double_arrow
ns-resize
sb_v_double_arrow
v_double_arrow
size_ver
2870a09082c103050810ffdffffe0204
00008160000006810000408080010102
# 48, 48

w-resize
e-resize
left_side
right_side
# 48, 48

n-resize
s-resize
top_side
bottom_side
# 48, 48

nesw-resize
fd_double_arrow
fcf1c3c7cd4491d801f1e1c78f100000
size_bdiag
48, 48

nwse-resize
size_fdiag
bd_double_arrow
c7088f0f3e6c8088236ef8e1e3e70000
48, 48
EOF;

$directory = '/home/Authenticode/Downloads/cursors/';

chdir($directory);

// foreach (explode("\n\n", $data) as $block) {
//     $names = explode("\n", $block);
//     $symlinks = array_slice($names, 1, -1);

//     $target = './' . current($names);

//     foreach ($symlinks as $link) {
//         $link = './' . $link;

//         if (file_exists($link)) {
//             unlink($link);
//         }

//         @symlink($target, $link);
//     }
// }

$filesToDelete = <<<EOF
ne-resize
sw-resize
top_right_corner
bottom_left_corner
48, 48

nw-resize
se-resize
top_left_corner
bottom_right_corner
48, 48
EOF;

chdir($directory);

foreach (explode("\n\n", $filesToDelete) as $block) {
    $symlinks = array_slice(explode("\n", $block), 0, -1);
  
    foreach ($symlinks as $link) {
        $link = './' . $link;

        if (file_exists($link)) {
            echo 'file exists.';
            unlink($link);
        }
    }
}
