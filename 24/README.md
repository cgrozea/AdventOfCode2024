https://adventofcode.com/2024/day/24 Part 2

After failing to model the constraint in Picat, I wrote a Picat script that converts the problem to a MiniZinc code model and solved that with Google OR Tools.

Eventually I corrected my Picat approach to part 2, the test there was for bitwise AND instead of adding binary-represented numbers. See part2.pi - a pure Picat solution.

Maybe interesting here also a generator I wrote to generate multiple instances of various sizes.

call: picat gen.pi N K|grep grep|cut -c6-

then the example generated models a circuit for adding two N bits numbers
where K gates have been pairwise swapped.



