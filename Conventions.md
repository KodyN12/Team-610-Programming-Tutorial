# Coding Conventions

Coding conventions are an important part of any project you are working on. With them, it makes it much easier for multiple people to collaborate on the same project, and it makes it easier to debug your code. Specifically with FRC programming, these are the conventions we use:<br>

<b>Variables</b>
<ul>
    <li>camelCase your variable names</li>
    <li>Do not use the this keyword in methods</li>
    <li>Instance variables begin with m_
        <ul>
            <li>Instance variables are generally used in Commands</li>
            <li>Ex: m_drivetrain</li>
        </ul>
    </li>
    <li>Static variables begin with s_
        <ul>
            <li>Static variables are generally used in Subsystems or places such as RobotContainer</li>
            <li>Ex: s_intakeInst</li>
        </ul>
    </li>
    <li>Access specifiers -> always default to private unless otherwise needed</li>
    <li>Always use doubles, never floats (extra values are important, especially in things such as PID)</li>
    <li>Constants
        <ul>
            <li>ALL CAPS, UNDERSCORES FOR SPACES</li>
            <li>Prefix <b>VAL_</b>: a value</li>
            <li>Prefix <b>PORT_</b>: a physical port number on the robot</li>
            <li>Prefix <b>CAN_</b>: a CAN bus ID</li>
            <li>Prefix <b>UNIT_</b>: conversion units (Ex. feet to meters)</li>
        </ul>
    </li>
</ul><br>

<b>Command Names</b>
<ul>
    <li>Prefix <b>T_</b>: teleoperated command</li>
    <li>Prefix <b>A_</b>: autonomous command</li>
    <li>Prefix <b>G_</b>: command groups</li>
    <li>Convention: <b>Prefix_Subsystem_action</b>
        <ul>
            <li>Ex. T_Intake_Up</li>
        </ul>
    </li>
</ul><br>

<b>Comments</b>
<ul>
    <li>Javadoc comments required</li>
    <li>More complicated code -> line-by-line comments</li>
</ul><br>

<b>Style</b>
<ul>
    <li>Ternary operators over if statements, where applicable</li>
    <li>Braces on the same line</li>
    <li>If-statements on one line, where applicable</li>
    <li>Declaration - Initialization not on the same line
        <ul>
            <li>Declare at class scope</li>
            <li>Initialize in the constructor</li>
        </ul>
    </li>
<ul><br>