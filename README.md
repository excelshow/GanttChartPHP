gantt_graph_php
===============

Class to generate gantt graph.

Use example:
<<<<<<< HEAD
```php
=======
```php 
>>>>>>> eca65bd63a4936a75542598d2f471d6b78b02b05
<?php
require /* PATH TO */ 'autoloader.php';

use GanttGraph\GanttGraph;

$array_data = array(
        array (
                'label' => 'Sub-Activitie',
                'series' => array (
                        array (
                                'label' => 'Sub-Activitie 1',
                                'allocations' => array (
                                        array (
                                                'label' => 'Task 1',
                                                'start' => '2013-09-15',
                                                'end' => '2013-09-29',
                                                'description' => 'Description x',
                                                'color' => '#00ff00',
                                        ),
                                        array (
                                                'label' => 'Task 2',
                                                'start' => '2013-09-04',
                                                'end' => '2013-09-06',
                                                'description' => 'Description y',
                                                'color' => '#0000ff',
                                        ),
                                        array (
                                                'label' => 'Task 3 (Example Conflict)',
                                                'start' => '2013-09-17',
                                                'end' => '2013-09-24',
                                                'description' => 'Description z',
                                                'color' => null, # color default
                                        ),
                                ),
                        ),
                ),
        ),
);

$gantt_graph = new GanttGraph( 'pt_BR' );

$gantt_graph->setData( $array_data )->render();
```
